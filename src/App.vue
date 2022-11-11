<template>
    <ToggleVue />
    <TodoVue />
    <TodoCompletedVue />
    <FetchTodo />
    <ParentComp />
    <CountVue />
    <ClassBinding />
    <RendringDec />
</template>

<script>
import ToggleVue from './components/ToggleVue.vue';
import TodoVue from './components/TodoVue.vue';
import TodoCompletedVue from './components/TodoCompletedVue.vue';
import FetchTodo from './components/FetchTodo.vue';
import ParentComp from './components/ParentComp.vue';
import CountVue from './components/CountVue.vue';
import ClassBinding from './components/ClassBinding.vue';
import RendringDec from './components/RendringDec.vue';

export default {
  name: 'App',
  components: {
    ToggleVue,
    TodoVue,
    TodoCompletedVue,
    FetchTodo,
    ParentComp,
    CountVue,
    ClassBinding,
    RendringDec
  }
}
</script>

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
