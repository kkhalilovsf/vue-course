<template>
  <li class="todo-list_item">
    <input type="checkbox" class="todo-list_native-checkbox" />
    <span class="todo-list_title">{{todo.title}}</span>
    <button type="button" class="todo-list_btn-notremove">&times;</button>
  </li>
</template>

<script>
export default {
  props: {
    todo: {
      type: Object,
      required: true,
    },
  },
};


</script>

<style scope lang="scss">
.todo-list_item {
  display: flex;
  align-items: center;
  margin-bottom: 0.5rem;
}
.todo-list_native-checkbox {
  margin-right: 0.5rem;
}
.todo-list_title {
  line-height: 0.7;
  font-size: 1.5rem;
}
.todo-list_btn-remove {
  margin-left: 0.5rem;
  background-color: #d81e1e;
  color: #fff;
  border: none;
  border-radius: 5px;
  font-size: 1.5rem;
  cursor: pointer;
}
</style>
