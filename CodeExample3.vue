<template>
  <ul>
    <li v-for="todo, index in thingsToDo" :key="index">
      {{ todo }}
    </li>
  </ul>
</template>

<script>
export default {
  name: 'CodeExample3',
  data() {
    return {
      thingsToDo: [
       'Acordar',
       'Tomar café',
       'Escovar os dentes'
      ]
    }
  }
}
</script>

<style scoped>

</style>
