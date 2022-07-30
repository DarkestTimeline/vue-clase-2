<template lang="en">
    <div>
        <h1>Sistemas Expertos</h1>

        <p></p>
        <input type="text" placeholder="Haga su consulta" v-model="pregunta"/>
        <p>Finalice su pregunta con un signo de interrogacion ?</p>

        <h1>{{pregunta}}</h1>
        <h2>{{respuesta}}</h2>
        <img :src="img" alt="GIF"/>
    </div>
</template>
<script>
export default {
    // Usar seccion data
    data() {
        return {
            pregunta: null,
            respuesta: null,
            img: null
        }
    },
    watch:{
        // Escuhar los cambios en la pregunta
        pregunta(value, oldvalue){
            console.log(value, oldvalue)
            // Si no incluye ?, no hacer nada
            if(!value.includes('?')) return
            // Si si incluye ?, llamar a un metodo con la respuesta
            this.getRespuesta()
        }
    },
    methods: {
        // Crear un metodo respuestas
        async getRespuesta(){
            const {answer, image} = await fetch('https://yesno.wtf/api').then(res => res.json())
            console.log(answer, image)

            // Vincular datos
            this.respuesta = answer
            this.img = image

        }
    },
}
</script>
<style lang="en">
    
</style>