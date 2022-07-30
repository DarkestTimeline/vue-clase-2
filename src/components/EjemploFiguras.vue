<template lang="en">
    <div>
        <h1>Seleccione a Pikachu:</h1>
        <form>
            <input type="radio" id="ditto" name="poke" value="ditto" @click="incorrecta">
            <label for="ditto"><img :src="ditto" alt=""/></label><br>

            <input type="radio" id="pika" name="poke" value="pika" @click="correcta">
            <label for="pika"><img :src="pika" alt=""/></label><br>

            <input type="radio" id="char" name="poke" value="char" @click="incorrecta">
            <label for="char"> <img :src="char" alt=""/></label><br>
        </form>

        <br>
        <h2>Respuesta {{res}}</h2>
    </div>
</template>
<script>
export default {
    data() {
        return {
            ditto: null,
            pika: null,
            char: null,
            res: "no seleccionada",
        }
    },
    methods: {
        async getDitto(){
            const ditto = await fetch('https://pokeapi.co/api/v2/pokemon/ditto').then(res => res.json())
            console.log(ditto.sprites.front_default)

            // Vincular datos
            this.ditto = ditto.sprites.front_default

        },
         async getPika(){
            const pika = await fetch('https://pokeapi.co/api/v2/pokemon/pikachu').then(res => res.json())
            console.log(pika.sprites.front_default)

            // Vincular datos
            this.pika = pika.sprites.front_default

        },
        async getChar(){
            const char = await fetch('https://pokeapi.co/api/v2/pokemon/charizard').then(res => res.json())
            console.log(char.sprites.front_default)

            // Vincular datos
            this.char = char.sprites.front_default

        },
        correcta(){
            //alert("Test")
            this.res = "correcta!"
        },
        incorrecta(){
            this.res = "incorrecta!"
        }
    },
    created() {
        this.getDitto()
        this.getPika()
        this.getChar()
    },
    
}
</script>
<style lang="en">
    
</style>