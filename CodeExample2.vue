<template>
  <div v-if="showText">
    {{ message }}
  </div>
</template>

<script>
export default {
  name: 'CodeExample2',
  data() {
    return {
      message: 'teste',
      showText: false
    }
  }
}
</script>

<style scoped>

</style>
