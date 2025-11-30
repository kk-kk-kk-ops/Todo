<script setup>
const Todos = [
  'buy milk',
  'buy pan',
  'buy ukiwa'
]
function addTodo() {
  alert('GO')
}

</script>

<template>
  <div class="container">
    <h1>Todos</h1>
    <ul>
      <li v-for="todo in Todos">{{ todo }}</li>

    </ul>
    <form @submit.prevent="addTodo">
      <input type="text">
      <button>Add</button>
    </form>
  </div>

</template>

<style scoped>
.container {
  width: 400px;
  margin: 0 auto;
}

h1 {
  font-size: 20px;
  border-bottom: 1px solid #000;
  padding-bottom: 8px;
}
</style>
