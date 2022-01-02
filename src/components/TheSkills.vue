<template>
    <div class= "skills">
        <h3 class="skills__title">Mis Habilidades</h3>
        <p class= "skills__text">Estas son algunas de mis habilidades. No tengo muchas porque no se olviden, solo tengo 5 años.</p>
    
        <div class= "skills__items">
            <div class="skills__item" v-for="habilidad in habilidades" :key="habilidad.id">
            <v-card-main 
             :titulo="habilidad.titulo"
             :contenido="habilidad.contenido"
             :color= "habilidad.color"/>
            </div>
        </div>
    </div>
</template>

<script>
     import VCardMain from "@/base/VCardMain.vue";

    export default {
         name:"TheSkills",
         data(){
            return{
                habilidades: [
                    {"id": 0, titulo: "Ordeñar Cabras", contenido: "Me gusta ordeñar cabras muy temprano por la mañana para poder desayunar.", color: "#54a0ff"},
                    {"id": 1, titulo: "Hacer Quesos y Manteca", contenido: "Me gusta cocinar mucho. Todo me enseñó mi abuelito.", color: "#5f27cd"},
                    {"id": 2, titulo: "Pastorear", contenido: "Cuando Pedro viene a buscar a mis cabras, nos vamos a la montaña y disfrutamos del paisaje.", color: "#f368e0"},
                    {"id": 3, titulo: "Jugar", contenido: "Me gusta jugar mucho, es una de mis pasiones.", color: "#01a3a4"},
                ]
            }
        },
        components:{
            VCardMain,
        },
        
    }
</script>

<style lang="css">
.skills{
    background: #222f3e;
    padding: 4em;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.skills__title {
    font-family: "Noto Serif", serif;
    color: white;
    margin-bottom: 1em;
    font-size: 24px;
}
.skills__text{
    font-family: "Ubuntu", sans-serif;
    color: white;
    margin-bottom: 1em;
}
.skills__items{
    display: grid;
    grid-template-columns:400px 400px;
    
}
.skills__item{
    margin: 10px;
}
</style>