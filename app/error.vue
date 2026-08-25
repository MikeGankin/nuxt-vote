<script setup lang="ts">
import UiButton from "~/components/UiButton.vue";

const handleGoHome = () => clearError({ redirect: "/" });
</script>

<template>
	<NuxtLayout>
		<div class="wrapper">
			<h1>404</h1>
			<span>Страница не найдена, вернитесь на главную страницу</span>
			<UiButton variant="primary" size="small" @click="handleGoHome">
				На главную
			</UiButton>
		</div>
	</NuxtLayout>
</template>

<style scoped>
.wrapper {
	box-sizing: border-box;
	display: flex;
	width: 100%;
	height: 100%;
	padding: 24px;
	flex-direction: column;
	justify-content: center;
	align-items: center;
}

h1 {
	margin: 0 0 24px;
	font-size: 120px;
	line-height: 1;
}

span {
	margin: 0 0 24px;
	color: var(--grey);
	text-align: center;
}
</style>
