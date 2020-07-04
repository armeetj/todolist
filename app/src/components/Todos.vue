<template>
    <div> 
        <h1>To-Dos</h1>
        <div v-bind:key="todo.id" v-for="todo in todos">
            <TodoItem />
        </div>
    </div>
</template>
<script>

import TodoItem from './TodoItem.vue'

export default {
    name: "Todos",
    components: {
        TodoItem
    },
    props: ["todos"]
}
</script>

<style scoped>

</style>