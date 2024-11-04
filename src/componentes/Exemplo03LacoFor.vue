<script setup>
    let nomes = ['Bianca','Apolo','Enzo','Heitor','Kiara']
</script>

<template>
    <ul>
        <li v-for="nome in nomes">{{ nome }}</li>
    </ul>
</template>

