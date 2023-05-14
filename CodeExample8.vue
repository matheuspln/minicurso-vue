<template>
  <div>
    <input type="text" v-model="firstName" placeholder="Nome do usuário">
    <br>
    <input type="text" v-model="lastName" placeholder="Sobrenome do usuário">
    <p class="red">O nome completo do usuário é {{ firstName + ' ' + lastName }}</p>
    <p class="green">O nome completo do usuário é {{ fullNameComputed }}</p>
  </div>
</template>

<script>
export default {
  name: 'CodeExample8',
  data() {
    return {
      firstName: '',
      lastName: '',
      fullName: '',
    }
  },
  computed: {
    fullNameComputed() {
      return this.firstName + ' ' + this.lastName
    }
  }
}
</script>

<style scoped>

.red {
  background-color: red;
  color: white;
}

.green {
  background-color: green;
  color: white;
}

</style>
