<template>
    <div class="componente">
        <h1>Componente de Renderização de Listas</h1>
        <p>Nome: {{ nome }}</p>
        <p v-show="cachorros.length === 0" >Não tem cachorro</p>
        <ul>
            <li v-for="cachorro in cachorros">
                nome: {{ cachorro.nome }} | Idade: {{ cachorro.idade }}
            </li>
        </ul>
    </div>
</template>

<script setup>


defineProps ({
    nome:String,
    cachorros:Array
})


</script>


<style scoped>
ul {
    margin: 0px;
    padding: 10px;
}

li{
    list-style: nome;
    text-align: center;
    font-size: large;
}

</style>