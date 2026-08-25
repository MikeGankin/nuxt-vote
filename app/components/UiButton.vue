<script setup lang="ts">
withDefaults(
	defineProps<{
		variant?: "primary" | "ghost";
		size?: "small" | "medium";
		fullWidth?: boolean;
		nativeType?: "button" | "submit" | "reset";
	}>(),
	{
		variant: "primary",
		size: "medium",
		fullWidth: false,
		nativeType: "button",
	},
);
</script>

<template>
	<button
		class="main-button"
		:class="[
			`main-button--${variant}`,
			`main-button--${size}`,
			{ 'main-button--full-width': fullWidth },
		]"
		:type="nativeType"
	>
		<slot />
	</button>
</template>

<style scoped>
.main-button {
	width: fit-content;
	border: none;
	background: transparent;
	font-size: inherit;
	font-weight: 500;
	border-radius: 30px;
	cursor: pointer;
	padding: 16px 32px;
}

.main-button--full-width {
	width: 100%;
}

.main-button--primary {
	background: var(--black);
	color: var(--white);
}

.main-button--ghost {
	border: 1px solid var(--black);
	color: var(--black);
}
</style>
