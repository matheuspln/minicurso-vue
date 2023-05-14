<template>
  <div>
    <input type="text" v-model="inputValue">
    <p>{{ inputValue }}</p>
  </div>
</template>

<script>
export default {
  name: 'CodeExample7',
  data() {
    return {
      inputValue: ''
    }
  }
}
</script>

<style scoped>

</style>
