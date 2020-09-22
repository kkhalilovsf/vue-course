<template>
  <div id="app">
    <TodoList 
      v-bind:todos="todos"
    />
  </div>
</template>

<script>
import TodoList from '@/components/TodoList';
export default {
  name: 'App',
  data() {
    return {
      todos: [
        {id: 1, title: 'Купить абрикосы', completed: false},
        {id: 2, title: 'Купить бананы', completed: false},
        {id: 3, title: 'Купить малину', completed: false}
      ]
    }
  },
  components: {
    TodoList: TodoList

  }
}
</script>

<style lang="scss">
* {
  outline: none;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 10px;
  display: flex;
  justify-content: center;
}
</style>
