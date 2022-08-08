<template lang="">
    <div>
        <h2>Matriz Nula</h2>
        <label for="filas">Filas: </label>
        <input type="number" name="filas" min="2" id="filas" v-model.number="filas" >
        <label for="col">Columnas: </label>
        <input type="number" name="col" min="2" id="col" v-model.number="col" >

        <p>{{matrizNula(this.col, this.filas)}}</p>
    </div>
</template>
<script>
export default {
    data() {
        return {
            filas: 2,
            col: 1
        }
    }, methods: {
        matrizNula(filas, col){
            const res = []
            for(let i = 0; i < filas; i++){
                if(!res[i]){
                    res[i] = []
                }
                for(let j = 0; j < col; j++){
                    res[i][j] = 0
                }
            }
            return res
        }
    },
    
}
</script>
<style>
    
</style>