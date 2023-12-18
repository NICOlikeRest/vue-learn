<template>
  <ul class="todo-main">
    <item-com 
      v-for="todoObj in todos" 
      :key="todoObj.id" 
      :todo="todoObj" 
      :checkTodo="checkTodo"
      :deleteTodo="deleteTodo"/>
  </ul>
</template>

<script>
import ItemCom from "./ItemCom.vue";
export default {
  name: "ListCom",
  components: { ItemCom },
  props:['todos', 'checkTodo', 'deleteTodo']
};
</script>

<style scoped>
/*main*/
.todo-main {
  margin-left: 0px;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding: 0px;
}

.todo-empty {
  height: 40px;
  line-height: 40px;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding-left: 5px;
  margin-top: 10px;
}
</style>