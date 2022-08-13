<template lang="en">
    <div>
        <h2>Matriz Inversa Metodo de Gauss Jordan</h2>
        <h3>Matriz A</h3>
       <span v-for="(item, index) in matrizA" :key="index">{{item}}<br></span>
        <h3>Matriz Inversa de Gauss Jordan</h3>
        <span v-for="(item, index) in matrizGJ()" :key="index">{{item}}<br></span>
    </div>
</template>
<script>
export default {
    data() {
        return {
            matrizA: [[1, 3], [2, 4]],
            matrizI: [[1, 0], [0, 1]]
        }
    }, methods: {
        matrizGJ(){
            const matrizA = this.matrizA;
            const matrizI = this.matrizI;
            return [matrizI, matrizA];
        }
    },
    
}
</script>
<style>
    
</style>