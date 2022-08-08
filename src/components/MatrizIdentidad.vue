<template lang="">
    <div>
        <h2>Matriz Identidad</h2>
        <label for="identidadSize">Tamaño: </label>
        <input type="number" name="identidadSize" min="2" id="identidadSize" v-model.number="identidadSize" >

        <p>{{matrizIdentidad(this.identidadSize)}}</p>
    </div>
</template>
<script>
export default {
    data() {
        return {
            identidadSize: 2
        }
    }, methods: {
        matrizIdentidad(identidadSize = 2){
            const res = []
            for(let i = 0; i < identidadSize; i++){
                if(!res[i]){
                    res[i] = []
                }
                for(let j = 0; j < identidadSize; j++){
                    if(i === j){
                        res[i][j] = 1
                    }else{
                        res[i][j] = 0
                    }
                }
            }
            return res
            }
        }

    }
</script>
<style>
    
</style>