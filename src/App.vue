<script setup>
import PrimeiroComponete from './components/PrimeiroComponete.vue';
import ComDados from './components/ComDados.vue'
import ComDadosReativosPrimitivos from './components/ComDadosReativosPrimitivos.vue';
import ComDadosReativosNaoPrimitivos from './components/ComDadosReativosNaoPrimitivos .vue';
import DataBinding from './components/DataBinding.vue';
import ComProps from './components/ComProps.vue';
import EscutaEvento from './components/EscutaEvento.vue';
import PropriedadesComputadas from './components/PropriedadesComputadas.vue';
import PropriedadesAssistidas from './components/PropriedadesAssistidas.vue';
import RenderizacaoCondicional from './components/RenderizacaoCondicional.vue';
import RenderizacaoListas from './components/RenderizacaoListas.vue';
import Slots from './components/Slots.vue';


const cachorrosdoJoao = [
  {nome:"Totó", idade:2},
  {nome:"Laika", idade:4},
  {nome:"Flor", idade:7}
]

</script>

<template>
  <header>Vue</header>
  <!-- <RenderizacaoListas nome="João" :cachorro="cachorrosdoJoao"/> A composição deixou de ser exibido no navegador por algum motivo -->
  <RenderizacaoCondicional nome="Maria" :qtde-dogs="0"/>
  <Slots/>
  <PropriedadesAssistidas/>
  <PropriedadesComputadas/>
  <ComDados/>
  <EscutaEvento/>
  <ComProps item="Biscoito " :preco="2.50"/>
  <DataBinding/>
  <ComDadosReativosPrimitivos/>
  <PrimeiroComponete/>
  <ComDadosReativosNaoPrimitivos/>
  
</template>

<style scoped>

</style>
