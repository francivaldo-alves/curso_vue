<template>
  <div>
    <h1>ola Vue</h1>
    <p>Meu nome é {{ nome }} e trabalho com {{ profissao }}</p>
    <MultiplosEventos />
    <Reutilizacao/>
    <Reutilizacao/>
    <Reutilizacao/>

    <Reutilizacao/>

    <Reutilizacao/>


  </div>
</template>

<script>
import MultiplosEventos from "./MultiplosEventos.vue";
import Reutilizacao from "@/components/Reutilizacao";
export default {
  components: {
    Reutilizacao,
    MultiplosEventos,
  },
  name: "PrimeiroComponete",
  data() {
    return {
      nome: "Francivaaldo",
      profissao: "Programador",
    };
  },
  
};
</script>