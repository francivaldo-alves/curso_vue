<template>
  <div>
    <form action="" @submit="enviarFormulario($event)">
      <div>
        <input type="text" v-model="name" />
      </div>
      <div>
        <input type="text" v-model="email" />
      </div>
      <div>
        <Subimit />
      </div>
    </form>
  </div>
</template>

<script>
import InputText from "./form/InputText.vue";
import Subimit from "./form/Subimit.vue";
export default {
  name: "Form",
  components: { InputText, Subimit },
  data() {
    return {
        name: '',
        email: ''
    };
  },
  methods: {
    enviarFormulario(e) {
      e.preventDefault();
      const name = this.name;
      const email = this.email;
      
       
      console.log("Formulário enviado");
      console.log ( " o Nome é" + name)
      console.log ( " o Nome é" + email)

      
    },
  },
};
</script>

<style scoped>
p {
  margin: 150;
}
</style>