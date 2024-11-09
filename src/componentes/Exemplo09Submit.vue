<script setup>

    function validaFormulario(){
        alert("Enviando formulário");
    }
</script>

<template>
    <!-- nesse caso o evento é passado no formulario e acontece atraves do type submit -->
    <form action="" @submit="validaFormulario">

        <input type="submit" value="Enviar formulario">
    </form>
</template>