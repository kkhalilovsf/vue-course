<template>
  <div>
    <ol class="todo-list">
      <TodoItem
        v-for="todo of todos" :key="todo.id"
        v-bind:todo="todo"
      />
    </ol>
  </div>
</template>

<script>
import TodoItem from "@/components/TodoItem";
export default {
  props: ['todos'],
  components: {
    TodoItem: TodoItem,
  },
};
</script>

<style scoped lang="scss">

  .todo-list {
    padding: 0;
    list-style-type: none;
  }

</style>