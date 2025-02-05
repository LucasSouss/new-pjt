<template>
    <div class="componente">
        <h1>Componentes Com Dados Reativos NÃO Primitivos</h1>
        <h2>Nome: {{ pessoa.nome }} | Idade: {{ pessoa.idade }}</h2>
        <button class="btt" v-on:click="mudarNome()" >Mudar Nome</button>
        <button class="btt" @click="fazerAniversario()">Fazer Aniversário</button>
        
    </div>
    
</template>

<!-- <script setup>
import {reactive} from 'vue'

const pessoa = reactive({nome: 'Ana', idade: 27})



function fazerAniversario() {
    pessoa.idade += 1
}

function mudarNome() {
    let newname = prompt('Digite um novo nome: ')
    pessoa.nome = newname

}

</script> -->

<script>
export default {
    data: function() {
          return {
            pessoa: {
              nome: 'Ana',
              idade: 27
            }
          }
    },
    methods: {
        fazerAniversario: function() {
            this.pessoa.idade += 1
        },
        mudarNome: function() {
            let newname = prompt('Digite um novo nome: ')
            this.pessoa.nome = newname

        }
    }
}



</script>

<style scoped>

</style>