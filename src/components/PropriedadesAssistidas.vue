<template>
    <div class="componente">
        <h1>Componente com Propriedades Assistidas</h1>
        <p>Idade: {{ idade }}</p>
        
        <input type="number" name="" id="" v-model="anoNascimento" min="1900">
        
        <input type="number" name="" id="" v-model="anoAtual" min="2000">
    </div>
</template>

<script setup>
import {ref} from 'vue'
// import {watch} from 'vue'
import { watchEffect } from 'vue'

const anoAtual = ref(2000)
const anoNascimento = ref(1900)
const idade = ref(0)

// watch(anoAtual, (ano) => {
//     idade.value = ano - anoNascimento.value
// })

// watch(anoNascimento, (ano)=> {
//     idade.value = anoAtual.value - ano
// })

watchEffect(() => {
    idade.value = anoAtual.value - anoNascimento.value
})


</script>