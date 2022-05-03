<template>
  <div>
      <button @click="$emit('mudarImagem')">Trocar Imagem do perfil</button>
  </div>
</template>

<script>
export default {
    name: 'MudarImagem',
    emits: ['mudarImagem']

}
</script>

<style>

</style>