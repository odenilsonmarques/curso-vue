<!-- js para declarar as variaveis que irao ser chamadas no templete -->
<script setup>
  let nome = 'Odenilson'
  let sobreNome = 'Araújo'
  let idade = 39


  let n1 = 300
  let n2 = 10
</script>



<!-- dentro da tag template vai o HTML -->
<template>
  <p>{{'Olá, ' + nome + ' ' + sobreNome + ' você tem ' + idade + ' anos'}}</p>

  <p>O resultado da soma é: {{n1+n2}}</p>

  <p>{{`O resultado da soma é: ${n1+n2}`}}</p>
</template>