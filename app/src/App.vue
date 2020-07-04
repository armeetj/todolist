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
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  body {
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.4;
  }
  .btn {
    display: inline-block;
    border: none;
    background: #555;
    color: #fff;
    padding: 7px 20px;
    cursor: pointer;
  }
  .btn:hover {
    background: #666;
  }
</style>
