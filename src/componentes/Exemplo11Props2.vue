<script setup>
    // obter props
    //chamando as propriedades
    const props = defineProps(['nome', 'idade', 'cidade', 'vetor', 'funcao']);


</script>


<template>
    <h1>Nome: {{ nome }}</h1>
    <h1>Idade: {{ idade }}</h1>
    <h1>Cidade: {{ cidade }}</h1>

    <ul>
        <li v-for="v of vetor">{{ v }}</li>
    </ul>

    <button @click="funcao">clique aqui</button>
</template>