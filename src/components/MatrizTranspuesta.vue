<template lang="">
    <div>
        <h2>Matriz Transpuesta</h2>
        <h3>Matriz A</h3>
        <span v-for="(item, index) in matrizA" :key="index">{{item}}<br></span>
        <h3>Mmatriz Transpuesta</h3>
        <span v-for="(item, index) in matrizT()" :key="index">{{item}}<br></span>
    </div>
</template>
<script>
export default {
    data() {
        return {
            matrizA: [[1, 0, 4], [0, 5, 0], [6, 0, -9]]
        }
    }, methods: {
        matrizT(){
            const matrizA = this.matrizA;
            return matrizA[0].map((col, i) => matrizA.map(row => row[i]));
        }
    },
    
}
</script>
<style>
</style>