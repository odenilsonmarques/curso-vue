<script setup>
    let exibir = true;

    let media = 7;
</script>

<template>
    <!-- O v-if verifica se o valor da variavel (exibir) é verdadeiro se for, exibe o texto, caso contrário nao exibe -->
    <h1 v-if="exibir"> Hello World !!</h1>

    <p v-if="media >= 7">Aprovado(a)</p>
    <p v-else-if="media >=5">Em exame</p>
    <p v-else>Reprovado(a)</p>
</template>