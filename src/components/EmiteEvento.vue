<template>
    <div class="componentes">
        <h1>Componente que emite Props</h1>
        <p>{{ item }} R${{ preco }}</p>
        <button class="btt" @click="adicionar">Adicionar ao Carrinho</button>
    </div>
</template>

<script>
import { defineProps, defineEmits } from "vue";

const props = defineProps ({
    item:String,
    preco:Number
})

const emit = defineEmits(["foiAdicionado"])

function adicionar() {
    emit("foiAdicionado", props.preco)
}

</script>