<template>
<div>
  <h2> Esta é a descrição da Pessoa: {{nome}} </h2>
  <Info/>
  <div>
      <h2> Formulario </h2>
      <Form/>
  </div>
 </div> 
</template>

<script>
import Form from './Form.vue';
import Info from './info.vue';
export default {
  name: "Pessoa",
  components: { Info, Form },
  data() {
    return {
      nome: "Francivaldo",
    };
  },
};
</script>

<style>
</style>