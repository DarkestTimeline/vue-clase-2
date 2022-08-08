<template lang="">
    <div>
        <h3>Matriz A</h3>
        <p>[ [ 1, -3 ], [ 2, 5 ] ]</p>
        <h3>Matriz B</h3>
        <p>[ [ 5, 4 ], [ 3, 8 ] ]</p>
        <h2>Suma de Matrices</h2>
        {{suma()}}
        <h2>Resta de Matrices</h2>
        {{resta()}}
    </div>
</template>
<script>
export default {
    data() {
        return {
            
        }
    }, methods: {
        suma(){
        const matrizA = [[1, -3], 
                         [2, 5]]
        const matrizB = [[5, 4],
                         [3, 8]]
        const res =[[], []]
        for (let i = 0; i < matrizA.length; i++) {
            for (let j = 0; j < matrizB.length; j++) {
                res[i][j] = matrizA[i][j] + matrizB[i][j]
            }
         }
        return res
        }, resta(){
            const matrizA = [[1, -3], 
                            [2, 5]]
            const matrizB = [[5, 4],
                            [3, 8]]
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