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
    this.lifeCycle()
  },
  mounted() {
     setTimeout(() => {
      this.nome = "Andesa";
    }, 2000);
    this.lifeCycle()
  },
  methods:{
    lifeCycle(){
      console.log("Exwcultou")
    }
  }
};
</script>

<style>
</style>