<template>
	<nav :style="{ background: '#333' }">
		<ion-icon name="menu"></ion-icon>
		<ul :stye="{ background: '#333' }">
			<li></li>
		</ul>
	</nav>
</template>

<script>
export default {
	name: 'NavigationMenu',
	props: ['navLinks', 'background'],
};
</script>

<style scoped lang="scss">
nav {
	height: 60px;
	width: 100%;
	color: white;
}

ion-icon {
	font-size: 64px;
}
</style>
