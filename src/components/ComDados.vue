<template>
    <div>
        <h1>Componentes com Dados</h1>
        <p>Nome: {{ nomeProduto }} - {{ codigoProduto }}</p>
        
    </div>
</template>


<style scoped>
div{
    border: 2px solid #d10000;
    background-color: #690000;
    border-radius: 15px;
    margin: 30px;
    padding: 40px;
    text-align: center;
}

</style>

<script setup>
const nomeProduto = "Apontador"
const codigoProduto = "#987"
</script>

<!-- <script>
//Options API
// export default {
//     data: function() {
//         return{
//             nomeProduto: "Caderno",
//             codigoProduto: "#321"
//         }
//     }
// }

// Composition API
// export default{
//     setup: function() {
//         const nomeProduto = 'Lapis'
//         const codigoProduto = '#789'
//         return {nomeProduto, codigoProduto}
//     }
// }
</script> -->