<template>
  <div>
    <li>
      <label class="todoList_label">
        <input class="todoList_input" type="checkbox" v-model="todo.completed" />
        <span>{{ todo.name }}</span>
      </label>
      <a href="#">
        <i class="fa fa-times"></i>
      </a>
    </li>
  </div>
</template>
<script setup>
const todo = defineProps(['id', 'name', 'completed'])
</script>
