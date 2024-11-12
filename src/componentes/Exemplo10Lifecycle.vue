<!-- Licecycle: São ações que podem acontecer em trÊs partes de um componente

1º Antes da criação

2º Durante a criação 

3º Após a criação -->

<script setup>
    //importações
    import {onMounted, ref} from 'vue';

    let texto = ref('Hello world');

    // lifecycle onMounted
    onMounted(() =>{
        setTimeout(() => {
            texto.value ="Alterando texto";
        }, 3000);
    });
</script>


<template>
    <h1>{{ texto }}</h1>
</template>