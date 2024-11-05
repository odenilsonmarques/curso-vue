<!-- 
 utilizando a diretiva v-model.
- A funcao dela é tabalhar com elementos de formulario.
- Nesse caso, ao digitar um texto no input o mesmo vai ser exibido na tela na tag de paragrafo
- Isso so é possivel deVIDO a importação do ref que garante a reatividade do conteudo pra essa situação
-->

<script setup>
    import { ref } from 'vue';
    let texto = ref('');
</script>


<template>
    <input type="text" v-model="texto">
    <p>{{ texto }}</p>
</template>