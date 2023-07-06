<template>
    <ul>
        <li v-for="(todo, idx) in todos" :key="idx">{{ todo.todo }}</li>
    </ul>
</template>

<script>
export default (await import('vue')).defineComponent({
    name: 'TodoList',
    props: {
        props: Array
    },
    mounted() {
        console.log(this.todos)
    }
})
</script>