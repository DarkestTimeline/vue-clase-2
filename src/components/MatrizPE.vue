<template lang="">
    <div>
        <h2>Producto Escala</h2>
        <h3>Matriz A</h3>
        <span v-for="(item, index) in matrizA" :key="index">{{item}}<br></span>
        <h3>Matriz Producto 3A</h3>
        <span v-for="(item, index) in matrizPE()" :key="index">{{item}}<br></span>
    </div>
</template>
<script>
export default {
    data() {
        return {
            matrizA: [[1, -3], [2, 5]]
        }
    }, methods: {
        matrizPE(){
            const matrizA = this.matrizA;
            const matrizR = [[], []]
            for(var i=0; i<2; i++){
                matrizR[0][i] = matrizA[0][i] * 3;
                matrizR[1][i] = matrizA[1][i] * 3;
            }
            return matrizR;
        }
    },
}
</script>
<style>
    
</style>