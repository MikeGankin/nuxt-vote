<script setup lang="ts">
import UiButton from "~/components/UiButton.vue";
</script>

<template>
	<div class="wrapper">
		<h1>404</h1>
		<span>Страница не найдена, вернитесь на главную страницу</span>
		<UiButton type="ghost">Главная страница</UiButton>
	</div>
</template>

<style scoped>
.wrapper {
	display: flex;
	height: 100%;
	width: 100%;
	flex-direction: column;
	justify-content: center;
	align-items: center;
}

h1 {
	margin-bottom: 24px;
	margin-top: 0;
	font-size: 120px;
}

span {
	margin-bottom: 64px;
	margin-top: 0;
}
</style>
