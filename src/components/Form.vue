<template>
 <div>
      <form action="">
      <div>
          <InputText/>
      </div>
       <div>
          <InputText/>
      </div>
      <div>
         <Subimit/>
      </div>

  </form>
 </div>
</template>

<script>
import InputText from './form/InputText.vue'
import Subimit from './form/Subimit.vue'
export default {
    name: 'Form',
  components: { InputText, Subimit },

}
</script>

<style>

</style>