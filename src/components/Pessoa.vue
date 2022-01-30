<template>
    <div>
        <h2>Está é a descrição da pessoa {{ nome }}</h2>
        <info :email="email" :esta_trabalhando=true />
        <Form />
    </div>
</template>

<script>
    import info from './info.vue'
    import Form from './Form.vue'
    export default {
        name: 'Pessoa',
        components: {
            info,
            Form
        },
        data() {
            return {
                nome: 'Vini',
                email:'vinislima@gmail.com'
            }
        }
    }
</script>