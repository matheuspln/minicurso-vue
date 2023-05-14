<template>
  <div :class="getClassName()">
    <p>Essa é uma demonstração de interpolação no {{ message }}</p>
    <button @click="changeClassName()">Mudar classe da div</button>
  </div>
</template>

<script>
export default {
  name: 'CodeExample6',
  data() {
    return {
      message: 'Vue JS',
      classToggle: true
    }
  },
  methods: {
    changeClassName() {
      this.classToggle = !this.classToggle
    },
    getClassName() {
      let className = this.classToggle ? 'class1' : 'class2'
      return className
    }
  }
}
</script>

<style scoped>

</style>
