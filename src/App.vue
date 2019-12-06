<template>
  <div id="app">
    <div class="container">
      <AddTodo />
      <FilterTodos />
      <Todos />
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  components: {
    Todos: () => import('@/components/Todos'),
    AddTodo: () => import ('@/components/AddTodo'),
    FilterTodos: () => import ('@/components/FilterTodos')
  }
}
</script>

<style>
body {
  /* font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif; */
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  line-height: 1.6;
  background: #e8f7f0;
}

.container {
  max-width: 1100px;
  margin: auto;
  overflow: auto;
  padding: 0 2rem;
}
</style>
