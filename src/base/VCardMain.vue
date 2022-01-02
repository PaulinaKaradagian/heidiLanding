<template>
    
   <div class= "main-card" :style= "{background: color}">
        <h4 class="main.card__title">{{titulo}}</h4>
        <p class="main-card__text">{{contenido}}</p>

    </div>
    
</template>

<script>
    export default {
        name: "VCardMain",
        props:{
            titulo: String,
            contenido: String,
            color: String,
        },
        
    }
</script>

<style lang="css">
.main-card{
    width: 300px;
    padding: 2em;
    color: white;
    margin: 10px;
    height: 100px;
}
.main-card__title{
    font-family: 'Noto Serif', serif;
    font-size: 20px;
    margin-bottom: 1em;
}
.main-card__text{
    font-family: 'Ubuntu', sans-serif;
    margin-top: 1em;
}

</style>