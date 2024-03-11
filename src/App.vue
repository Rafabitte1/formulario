<script setup>
    const cidade = [
  'São Paulo',
  'Rio de Janeiro',
  'Belo Horizonte',
  'Salvador',
  'Fortaleza',
  'Curitiba',
  'Manaus',
  'Recife',
  'Porto Alegre',
  'Brasília',
];

let cidade2 =
[
  'São Paulo',
  'Rio de Janeiro',
  'Belo Horizonte',
  'Salvador',
  'Fortaleza',
  'Curitiba',
  'Manaus',
  'Recife',
  'Porto Alegre',
  'Brasília',
];
cidade2.sort((a,b) =>{
  if(a>b){
  return -1;
  } if(a<b)
  return 1;
  return 0;
})
</script>
<template>
  <div>
  <h1>execicio1</h1>
 <ul>
  <li v-for="(cidade,index) in cidade" :key="index">{{ cidade }}</li>
 </ul>
  </div>
  <div>
    <h1>exercicio2</h1>
    <ul>

      <li v-for="(cidade2,index) in cidade2 " :key="index">{{ cidade2 }}</li>
    </ul>

  </div>
</template>