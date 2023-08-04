<template>
	<div>
		<input v-model="todoValue" type="text">
		<button>Compo</button>
	</div>
</template>

<script>

export default (await import('vue')).defineComponent({
	name: 'AddNewCompo',
	data() {
		return {
			todoValue: "compo"
		}
	}
})
</script>