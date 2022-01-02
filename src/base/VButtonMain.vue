<template>
    <a class= "main-btn" href="#" :style="{background: colorFondo, color: colorFondo}">
        {{text}}
    </a>
</template>

<script>
    export default {
        name: "VButtonMain",
        props: {
            text: String,
            colorTexto: String,
            colorFondo: String,
        },
        
    }
</script>

<style>

.main-btn{
    padding: 7px 20px;
    font-family: 'Ubuntu', sans-serif;
    border: 1px solid;
    text-decoration: none;
    margin: 5px;
}

</style>