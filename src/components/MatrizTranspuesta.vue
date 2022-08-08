<template lang="">
    <div>
        <h2>Matriz Transpuesta</h2>
        <h3>Matriz A</h3>
        <p>[ [ 1, 0, 4 ], [ 0, 5, 0 ], [ 6, 0, -9 ] ]</p>
        <h3>Mmatriz Transpuesta</h3>
        <p>{{matrizT()}}</p>
    </div>
</template>
<script>
export default {
    data() {
        return {
        }
    }, methods: {
        matrizT(){
            const matrizA = [[1, 0, 4], [0, 5, 0], [6, 0, -9]];
            return matrizA[0].map((col, i) => matrizA.map(row => row[i]));
        }
    },
    
}
</script>
<style>
</style>