<script setup lang="ts">
defineProps<{
	type?: string
}>()
</script>

<template>
	<button
			class="main-button"
			:class="type === 'primary' ? 'primary' : 'ghost'"
			type="button"
	>
		<slot></slot>
	</button>
</template>

<style scoped>
.main-button {
	padding: 16px;
	background: transparent;
	width: fit-content;
	border: none;
	font-size: 16px;
	font-weight: 700;
	border-radius: 8px;
	cursor: pointer;
}

.primary {
	background: var(--black);
	color: var(--white);
}

.ghost {
	border: 1px solid var(--black);
	color: var(--black);
}
</style>