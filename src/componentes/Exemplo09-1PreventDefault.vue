
<!-- -Nese caso estamos usando o preventDefault ele impede que ao clicar em ok para fechar a mensagem do alert a página seja direcoinada
para a url informada no action. -->


<!-- -Essa recurso é importante ser usado quando desejamos validar todo o formulario ou seja garantir que todos os campos sao preenchido
ante do envio do formuario -->


<script setup>

    function validaFormulario(event){
        alert("Formulário enviado");
        event.preventDefault();
    }
</script>

<template>
    <form action="https://odenilsonmarques.github.io/portfolio/#start" @submit="validaFormulario">
        <input type="submit" value="Enviar formulário">
    </form>
</template>