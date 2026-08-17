<script setup lang="ts">

import UiButton from "~/components/UiButton.vue";
</script>

<template>
	<div class="wrapper">
		<h1>404 ошибка</h1>
		<span>Страница не найдена, попробуйте перейти на главную страницу</span>
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
}

span {
	margin-bottom: 64px;
	margin-top: 0;
}
</style>