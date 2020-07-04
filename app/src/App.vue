<template>
  <div id="app">
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>

import Todos from './components/Todos'

export default {
  name: 'App',
  components: {
    Todos
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          title: 'Take a shower',
          completed: false
        },
        {
          id: 2,
          title: 'Brush teeth',
          completed: false
        },
        {
          id: 3,
          title: 'Eat breakfast',
          completed: false
        },
        {
          id: 3,
          title: 'Wake up',
          completed: true
        }
      ]
    }
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
