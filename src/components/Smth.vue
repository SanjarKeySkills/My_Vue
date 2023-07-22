<template>
    <span>
        Lorem where are you?
    </span>

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