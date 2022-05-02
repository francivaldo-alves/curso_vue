<template>
  <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
export default {
  name: "LyfeCycle",
  data() {
    return {
      nome: "Ainda não sei",
    };
  },
  created() {
    setTimeout(() => {
      this.nome = "Fran";
    }, 1000);
  },
  mounted() {
     setTimeout(() => {
      this.nome = "Andesa";
    }, 2000);
  },
};
</script>

<style>
</style>