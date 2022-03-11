<script setup>
import TodoHeader from './components/TodoHeader.vue'
import TodoTitle from './components/TodoTitle.vue'
import TodoInput from './components/TodoInput.vue'
import TodoController from './components/TodoController.vue'
import TodoList from './components/TodoList.vue'
import TodoFooter from './components/TodoFooter.vue'

</script>

<template>
  <TodoHeader></TodoHeader>
  <TodoTitle></TodoTitle>
  <TodoInput></TodoInput>
  <TodoController></TodoController>
  <TodoList></TodoList>
  <TodoFooter></TodoFooter>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
