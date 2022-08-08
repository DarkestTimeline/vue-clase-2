<template lang="">
    <div>
        <h2>Producto Escala</h2>
        <h3>Matriz A</h3>
        <p>[ [ 1, -3 ], [ 2, 5 ] ]</p>
        <h3>Matriz Producto 3A</h3>
        <p>{{matrizPE()}}</p>
    </div>
</template>
<script>
export default {
    data() {
        return {
            
        }
    }, methods: {
        matrizPE(){
            const matrizA = [[1, -3], 
                             [2, 5]];
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