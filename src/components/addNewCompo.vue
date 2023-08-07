<template>
	<div>
		<input v-model="todoValue" type="text">
		<button>App2</button>
	</div>
</template>

<script>

export default (await import('vue')).defineComponent({
	name: 'AddTodo',
	data() {
		return {
			todoValue: "assdd"
		}
	}
})
</script>