<template>
  <ul v-if="showList">
    <li v-for="todo, index in thingsToDo" :key="index">
      {{ todo }}
    </li>
  </ul>
  <button @click="hideList()">Mostrar/esconder lista</button>
</template>

<script>
export default {
  name: 'CodeExample4',
  data() {
    return {
      thingsToDo: [
       'Acordar',
       'Tomar café',
       'Escovar os dentes'
      ],
      showList: true
    }
  },
  methods: {
    hideList() {
      this.showList = !this.showList
    }
  }
}
</script>

<style scoped>

</style>
