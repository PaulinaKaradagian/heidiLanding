<template>
    <div class="personal-data">
         <div class="personal-data__left">
             <div class= "personal-data__left__content">
                 <span class="personal-data__left__content__text">Hola!</span>
                 <h3 class="personal-data__left__content__name">Soy Heidi</h3>
                     <p class="personal-data__left__content__description"> Me llevaron a vivir con mi abuelo a los Alpes. Después vino mi tía Dette y me llevó a Alemania con los Sessemann.Por suerte pude volver a mis amados Alpes.
                    </p>
                     
                    <v-button-main class="btn"
                    text= "Contactar"
                   
                    />
                </div>
                 
            </div>
             
         <div class= "personal-data__right">
                <img class="personal-data__right__img" src= "../assets/heidi.png" alt="Heidi Dancing">
         </div>
    </div>
</template>

<script>
    import VButtonMain from "@/base/VButtonMain.vue";
    export default {
        name:"ThePersonalData",
        components: {
            VButtonMain,
        },
    }
</script>

<style lang="css">
@import url('https://fonts.googleapis.com/css2?family=Noto+Serif:wght@700&family=Ubuntu:wght@300&display=swap');

.personal-data{
    display: flex;
    border: 1px solid;
}
.personal-data__left{
    background: #222f3e;
    width: 60%;
    justify-content: center;
    align-items: center;
    display: flex;

}
.personal-data__left__content{
    width: 300px;
    color: white;

}
.personal-data__left__content__text{
    font-size: 14px;
    font-family: 'Ubuntu', sans-serif;
    margin-bottom: 10px;
}
.personal-data__left__content__name{
    font-size: 24px;
    font-family: 'Noto Serif' , serif;
    margin-bottom: 10px;
    color: #54a0ff;
}
.personal-data__left__content__description{
    font-size: 14px;
    font-family: "Ubuntu", sans-serif;
    margin-bottom: 2em;
}
.personal-data__right{
    width: 40%;
    background: #54a0ff;
    
}
.personal-data__right__img{
    position: relative;
    width: 200px;
    left: -110px;
}
.btn{
    background:#222f3e;
    color:#54a0ff;
}
</style>