<template>
<div>
      <img :src="avatar" :alt="descricao">
      <Mudarimagem @mudar-imagem="trocarImagem"/>
</div>
</template>

<script>
import Mudarimagem from './Mudarimagem.vue'
export default {
    name: 'Picture',
    components: { Mudarimagem },
    data(){
        return {
            avatar : "/img/avatar.png",
            descricao: 'Francivaldo Alves',
        }
    },
    methods:{
        trocarImagem(){
            this.avatar = "/img/avatar2.png"
            console.log("opa")

        }
    }

}
</script>

<style>

</style>