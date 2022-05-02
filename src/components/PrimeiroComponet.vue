<template>
  <div>
    <h1>ola Vue</h1>
    <p> Meu nome é {{nome}} e trabalho com {{profissao}}</p>
  </div>
</template>

<script>
export default {
  name: "PrimeiroComponete",
  data() {
    return {
      nome: "Francivaaldo",
      profissao : "Programador"
    };
  },
};
</script>