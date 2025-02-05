<template>
    <div class="componente">
        <h1>Componentes Com Dados Reativos Primitivos</h1>
        <h2>Nome: {{ nome }} | Idade: {{ idade }}</h2>
        <button class="btt" v-on:click="mudarNome()" >Mudar Nome</button>
        <button class="btt" @click="fazerAniversario()">Fazer Aniversário</button>
        
    </div>
    
</template>

<script setup>
import {ref} from 'vue'

const nome = ref('Maria')
const idade = ref(27)

function fazerAniversario() {
    idade.value += 1
}

function mudarNome() {
   let newnome = prompt('Digite um novo nome: ')
   nome.value = newnome

}

</script>

<style scoped>

</style>