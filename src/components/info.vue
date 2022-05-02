<template>
  <div>
    <p v-if="esta_trabalhando">Estou Trabalhando no momento</p>
    <p v-else>Estou em buscas se novas opurtunidades</p>
    <p>utilizo as seguintes tecnologias para back-end </p>
    <ul > 
      <li v-for="(backend, index) in backends" :key=index>{{backend}}</li>
      
    </ul>
    <p>Utilizo as seguintes tecnologias para front-end</p>
    <ul>
      <li v-for="frontend in frontends" :key="frontend.id">{{frontend.language}}</li>
    </ul>
    <div>
      <button @click="showEmail">{{textoBotao}}</button>

    </div>
    <p v-show="mostrar_email">Mandei email para {{ email }}</p>
    <p class="teste">
      para acessar o meu portifólio
      <a v-bind:href="meu_link" target="_blank"> basta clicar aqui</a>
    </p>
    <Picture/>
  </div>
</template>

<script>
import Picture from "./Picture.vue";
export default {
  name: "Info",
  components: { Picture },
  data() {
    return {
      esta_trabalhando: false,
      mostrar_email: false,
      email: "francivaldo@souza.com.br",
      meu_link: "https://www.google.com",
      textoBotao : "Mostrar email",
      backends:['Java','PHP','Python'],
      frontends:[
        {id:1, language: 'HTML'},
        {id:2, language:'CSS'},
        {id:3, language:'VueJS'}
      ]

    };
  },
  methods:{
    showEmail(){
      this.mostrar_email =!this.mostrar_email;
      console.log(this.mostrar_email);
      if(!this.mostrar_email){
        this.textoBotao = "Mostrar e-mail"
      }else{
        this.textoBotao ='Esconder Email'
      }

    }
  }
};
</script>

<style>
.paragrafo-pai{
  color: red;
}
</style>