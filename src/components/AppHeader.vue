<template>
    <header>
        <h1>{{ appTitle }}</h1>
				<button @click="changeTitle">변경</button>
    </header>
</template>

<script>
	export default {
			props: ['appTitle'],
			methods: {
				changeTitle(){
					this.$emit('change');
				}
			}
	}
</script>

<style>
</style>