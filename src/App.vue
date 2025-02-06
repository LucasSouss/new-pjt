<script setup>
import PrimeiroComponete from './components/PrimeiroComponete.vue';
import ComDados from './components/ComDados.vue'
import ComDadosReativosPrimitivos from './components/ComDadosReativosPrimitivos.vue';
import ComDadosReativosNaoPrimitivos from './components/ComDadosReativosNaoPrimitivos .vue';
import DataBinding from './components/DataBinding.vue';
import ComProps from './components/ComProps.vue';

</script>

<template>
  <header>Abobora</header>
  <ComDados/>
  <ComProps item="Biscoito " :preco="2.50"/>
  <DataBinding/>
  <ComDadosReativosPrimitivos/>
  <PrimeiroComponete/>
  <ComDadosReativosNaoPrimitivos/>
  
</template>

<style scoped>

</style>
