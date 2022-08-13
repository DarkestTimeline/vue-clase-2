<template lang="">
    <div>
        <h2>Potencia de matriz</h2>
        <h3>Matriz A</h3>
        <span v-for="(item, index) in matrizA" :key="index">{{item}}<br></span>
        <h3>Matriz Potencia</h3>
        <span v-for="(item, index) in matrizP()" :key="index">{{item}}<br></span>
    </div>
</template>
<script>
export default {
    data() {
        return {
            matrizA: [[1, -3], [2, 5]]
        }
    }, methods: {
        matrizP(){
            const matrizA = this.matrizA;
            const matrizR = [[], []]
            matrizR[0][0] = (matrizA[0][0] * matrizA[0][0]) + (matrizA[0][1] * matrizA[1][0]);
            matrizR[0][1] = (matrizA[0][0] * matrizA[0][1]) + (matrizA[0][1] * matrizA[1][1]);
            matrizR[1][0] = (matrizA[1][0] * matrizA[0][0]) + (matrizA[1][1] * matrizA[1][0]);
            matrizR[1][1] = (matrizA[1][0] * matrizA[0][1]) + (matrizA[1][1] * matrizA[1][1]);
            return matrizR
        }
    },
    
}
</script>
<style>
    
</style>