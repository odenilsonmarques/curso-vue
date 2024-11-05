<!-- 
 utilizando a diretiva :class nesse caso nao tem v-class.
- A funcao dela é permitir a estilização do texto
-->


<script setup>
    let validacao = false
</script>

<!-- css -->
<style>
    .ok{
        color: darkgreen;
    }

    .falha{
        color:brown;
    }
</style>


<!-- Html -->
 <template>
    <!-- usamos um if ternario para aplicar a validacao dependendo do valor da variavel true u false -->
    <p :class="validacao ? 'ok' : 'falha'">utilizando a diretiva class</p>
 </template>