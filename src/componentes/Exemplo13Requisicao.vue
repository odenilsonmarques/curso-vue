<script setup>

import { onMounted, ref } from 'vue';

//vetor contendo ppostagens
let vetor = ref([]);

onMounted(() =>{
    // usando o fetch para fazer a requisição
    fetch('https://jsonplaceholder.typicode.com/posts')

    // convertendo os dados da requisicação para json
    .then(retorno => retorno.json())

    // atribuindo o json para a variael vetor
    .then(retorno => vetor.value = retorno)

});

</script>


<template>
    <h1>Requisições</h1>

    <!-- exibido resultado da reuisição -->
     <table>
        <tr>
            <td><strong>User</strong></td>
            <td><strong>#</strong></td>
            <td><strong>Title</strong></td>
            <td><strong>Body</strong></td>
        </tr> 
        <tr v-for="v in vetor">
            <td>{{ v.userId }}</td>
            <td>{{ v.id }}</td>
            <td>{{ v.title }}</td>
            <td>{{ v.body }}</td>
        </tr>
     </table>

</template>