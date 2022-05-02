<template>
  <div>
       <p v-if="esta_trabalhando"> Estou Trabalhando no momento </p>
       <p v-else> Estou em buscas se novas opurtunidades</p>
   <p> utilizo as seguintes tecnologias: </p>
   <ul>
       <li> Java</li>
       <li> PHP </li>
       <li> Python </li>

   </ul>
   <p v-show="mostrar_email"> Mandei email para {{email}}</p>

  </div>
</template>

<script>
export default {
    name: 'Info',
    data(){
        return{
            esta_trabalhando: false,
            mostrar_email: false,
            email:'francivaldo@souza.com.br'
        }
    }
    

}
</script>

<style>

</style>