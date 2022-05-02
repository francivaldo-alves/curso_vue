<template>
  <div>
  <Header/>

    <PrimeiroComponete/>
    <p class="paragrafo-pai"> os dados do APP é {{testando}}</p>
    <LifeCycle/>
    <Pessoa/>
  </div>
 
</template>

<script>
import Header from './components/Header.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'
import PrimeiroComponete from './components/PrimeiroComponet.vue'

export default {
  name: 'App',
  components:{
    PrimeiroComponete,
    LifeCycle,
    Pessoa,
    Header
  },
  data(){
    return{
      testando : 'TESTE',
    }
  }

}

</script>
<style>
body{
  background-color: #333;
  color: #FFF;
}
a {
  color: red;
}
.teste{
  background-color: #000;
}

</style>
