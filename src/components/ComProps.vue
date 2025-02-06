<template>
    <div class="componente">
        <h1>Componente Com Props</h1>
        <p>{{ item }}(R$ {{ preco }})</p>
    </div>
</template>

<script setup>
import { defineProps } from 'vue';

defineProps({
    item:String,
    preco:Number
})

</script>