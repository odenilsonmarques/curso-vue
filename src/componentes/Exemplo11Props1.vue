<!-- props é usada para passar dados de um componente pai para um componente filho. 
 Isso permite que o componente filho receba dados(informações estáticas, variaveis e funçõe) externos, tornando-o mais reutilizável e dinâmico. 
 
 para execeutar devemos chamar no app.vue apenas o props pai no caso(Exemplo11props1)
 
 -->


<script setup>

    // importando componente 
    import Exemplo11Props2 from './Exemplo11Props2.vue';


    //props com variaveis
    let cidade = 'São José de Ribamar';

    //usando um vetor
    let clubes = ['Flamengo', 'Corinthians', 'Botafogo', 'Palmeiras'];


    //usando funcao
    function mensagem(){
        alert('Usando funcção com props');
    }


</script>


<template>
    <!-- referenciando ao componente filho -->
     <!-- dentro da tag que faz referencia ao componente filho, passamos as propridades. Lembrando que pode ser qualquer nome -->
      <!-- a refencia a variavel nesse caso tem que ser usando os dois pontos. dessa forma o valor ficar dinamico, ou seja assim que eu trocar
      o valor este é exibido  -->
      <!-- para refenciar o vetor e a variaveis pode ser usado qualquer nome, somente o valor devem ser igual
      por exemplo declarei no vetor o nome de clubes na tag chamei de vetor, mas o valor ficou clubes -->

    <Exemplo11Props2 nome="Odenilson" idade="37" :cidade="cidade" :vetor="clubes" :funcao="mensagem">

    </Exemplo11Props2>
</template>