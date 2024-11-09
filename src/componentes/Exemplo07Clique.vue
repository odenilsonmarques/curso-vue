<script setup>

    function mensagem(){
        alert("Trabalhando com evento de clique");
    }

</script>

<template>
    <!-- esse apenas um do eventos de clique, existe vários -->
    <button @click="mensagem">Clique aqui</button>
</template>