<template lang="">
    <div>
        <h3>Matriz A</h3>
        <span v-for="(item, index) in matrizA" :key="index">{{item}}<br></span>
        <h3>Matriz B</h3>
        <span v-for="(item, index) in matrizB" :key="index">{{item}}<br></span>
        <h2>Suma de Matrices</h2>
        <span v-for="(item, index) in suma()" :key="index">{{item}}<br></span>
        <h2>Resta de Matrices</h2>
        <span v-for="(item, index) in resta()" :key="index">{{item}}<br></span>
    </div>
</template>
<script>
export default {
    data() {
        return {
            matrizA: [[1, -3], [2, 5]],
            matrizB: [[5, 4], [3, 8]],
            items: [{ message: 'Foo' }, { message: 'Bar' }]
        }
    }, methods: {
        suma(){
        const matrizA = this.matrizA
        const matrizB = this.matrizB
        const res =[[], []]
        for (let i = 0; i < matrizA.length; i++) {
            for (let j = 0; j < matrizB.length; j++) {
                res[i][j] = matrizA[i][j] + matrizB[i][j]
            }
         }
        return res
        }, resta(){
            const matrizA = this.matrizA
            const matrizB = this.matrizB
            const res =[[], []]
            for (let i = 0; i < matrizA.length; i++) {
                for (let j = 0; j < matrizB.length; j++) {
                    res[i][j] = matrizA[i][j] - matrizB[i][j]
                }
            }
            return res
        }
    }
}
</script>
<style>
</style>