<template>
	<div class="default-layout">
		<aside class="aside-menu">
				<Icon size="24" name="i-lucide-house" />
				<Icon size="24" name="i-lucide-door-open" />
		</aside>

		<main class="main">
			<slot />
		</main>
	</div>
</template>

<style scoped>
.main {
	grid-area: main;
}

.default-layout {
	display: grid;
	min-height: 100%;
	grid-template-columns: min-content auto;
	grid-template-areas:
	"aside main"
;
}

.aside-menu {
	padding: 42px 28px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
	grid-area: aside;
	border-right: 1px solid hsla(0, 0%, 90%, 1);
}
</style>
