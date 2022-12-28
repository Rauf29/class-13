<template>
  <ul >
    <li v-for="todo in todos">{{todo.title}}</li>
  </ul>
</template>

<script>
export default {
  name: "About",
  data() {
    return {
      todos: []
    }
  },
  mounted() {
    fetch('https://jsonplaceholder.typicode.com/todos')
        .then(response => response.json())
        .then(json => this.todos =json)
  }
}
</script>

<style scoped>

</style>