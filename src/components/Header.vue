<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projeto</a></li>
        <li><a href="#">Contato</a></li>
        <li v-if="esta_logado"><a href="#">Meu Perfil</a></li>
    </ul>    
</template>

<script>
export default {
    name: 'Header',
    props: ["esta_logado"]
}   
</script>

<style scoped>
    ul {
        list-style: none;
        display: flex;
        background-color: #999;
    }

    li {
        margin-right: 10px;
    }

    a {
        color: #ddd;
        text-decoration: none;
        transition: .5s;
    }

    a:hover {
        color: #00ced1;
    }
</style>
