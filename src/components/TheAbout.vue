<template>
    <div class="about">
        <div class= "about__content">
            <div class= "about__content__left">
                <img class= "about__content__left__img" src= "../assets/heidi2.jpg" alt= "Heidi">
            
            
            
            </div>
            <div class= "about__content__right">
                <h3 class= "about__content__right__title">Sobre mi</h3>
                <p class= "about__content__right__text"> Yo era muy feliz con mi abuelito, viviendo en mis queridos Alpes. Jugaba con las cabras y con mi mejor amigo, Pedro. Él tiene una abuelita a quien yo quiero mucho. Pensaron que podía educarme mejor en Alemania, pero se equivocaron.</p>
                <div class= "about__content__right__ctrls">
                    <v-button-main class="btn1"
                        text= "Linkedin"
                        />
                    
                    <v-button-main class= "btn2"
                        text= "Github"
                        />
                </div> 
            
            
            </div>
        
        
        
        </div>

    </div>
</template>

<script>
    import VButtonMain from "@/base/VButtonMain.vue"

    export default {
        name: "TheAbout",
        components: {
            VButtonMain,
        }
    }
</script>

<style lang="css">
.about{
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 5em;
    padding-bottom: 5em;
    background: #222f3e;
    opacity: 0.95;
}
.about__content{
    width: 50%;
    display:flex;
    justify-content: center;
    align-items: center;
}
.about__content__left{
    border: 1px solid #54a0ff;
    width: 150px;
    height: 200px;
    margin-right: 3em;
}
.about__content__left__img{
    width: 100%;
    height: 100%;
    position: relative;
    left: 20px;
    top: -20px;
}
.about__content__right{
    width: 50%;
    display: block;
    color: white;
}

.about__content__right__title{
    font-family: 'Noto Serif', serif;
    font-size: 20px;
    border-bottom: 1px solid #54a0ff;
    margin-bottom: 1em;
    padding-bottom: 1em;
}

.about__content__right__text{
    font-family: 'Ubuntu', sans-serif;
    font-size: 15px;
    margin-bottom: 1.5em;
}
.btn1{
    background: #54a0ff;
    color: #222f3e;
    
}
.btn2{
    background: #222f3e;
    color: #54a0ff;
    
}
</style>