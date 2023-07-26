<template>
    <div>
        <input v-model="todoValue1" type="text">
        <button>App</button>
    </div>
</template>

<script>

export default (await import('vue')).defineComponent({
    name: 'AddTodo',
    data() {
        return {
            todoValue: "123"
        }
    }
})
</script>