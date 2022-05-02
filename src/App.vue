<template>
  <div>
    <PrimeiroComponete/>
    <LifeCycle/>
    <Pessoa/>
  </div>
 
</template>

<script>
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'
import PrimeiroComponete from './components/PrimeiroComponet.vue'

export default {
  name: 'App',
  components:{
    PrimeiroComponete,
    LifeCycle,
    Pessoa
  }

}


</script>
