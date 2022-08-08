<template lang="en">
    <div>
        <h2>Matriz Inversa Metodo de Gauss Jordan</h2>
        <h3>Matriz A</h3>
        <p>[ [ 1, 0, 4 ], [ 0, 5, 0 ], [ 6, 0, -9 ] ]</p>
        <h3>Matriz Inversa de Gauss Jordan</h3>
        <p>{{matrizGJ()}}</p>
    </div>
</template>
<script>
export default {
    data() {
        return {
            
        }
    }, methods: {
        matrizGJ(){
            const matrizA = [[1, 3], 
                             [2, 4]];
            const matrizI = [[1, 0], 
                             [0, 1]];
            return [matrizI, matrizA];
        }
    },
    
}
</script>
<style>
    
</style>