<script setup>

    function mensagem(){
        alert("Executando a função")
    }

</script>


<template>
    <!-- o objetivo dessa funçõa é exibir a mensagem quando a letra R for pressionada. No entato, pode servir para outros fins -->
    <input type="text" @keyup.r="mensagem">
</template>
