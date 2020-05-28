<template>
  <div>
    <ul>     
      <TodoItem 
        v-for="todo of todos"
        v-bind:todo="todo"
      />
    </ul>
  </div>
</template>

<script>
import TodoItem from '@/components/todo-item'
export default {
  props: ['todos'],
  components: {
    TodoItem
  }
}
</script>