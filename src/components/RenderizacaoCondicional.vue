<template>
    <div class="componente">
        <h1>Componente com Renderização Condicional</h1>
        <p>Nome: {{ nome }}</p>
        <p v-if="qtdeDogs === 0">Não tem cachorro</p>
        <p v-else-if="qtdeDogs === 1" >Tem um cachorro</p>
        <p v-else>Tem muitos cachorro</p>
    </div>
</template>

<script setup>
import { defineProps } from 'vue';

defineProps({
    nome:String,
    qtdeDogs:Number
})
</script>