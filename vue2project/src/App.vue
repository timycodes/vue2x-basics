<template>
	<div id="app">
		<NavigationMenu></NavigationMenu>
		<div class="girl-container">
			<img class="face" alt="female face" src="./assets/girl.jpg" />
		</div>
		<img class="vuelogo" alt="vue logo" src="./assets/logo.png" />
		<router-view></router-view>
	</div>
</template>

<script>
import NavigationMenu from '@/components/NavigationMenu';

export default {
	name: 'App',
	components: {
		NavigationMenu,
	},
};
</script>

<style lang="scss">
@import 'https://unpkg.com/ionicons@4.2.2/dist/css/ionicons.min.css';

* {
	box-sizing: border-box;
	padding: 0;
	margin: 0;
}

body {
	margin: 0;
}

#app {
	font-family: 'Roboto', Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
}

.girl-container {
	display: flex;
	align-items: center;
	justify-content: center;
	border: 2px solid black;
	background-color: black;
}
.face {
	display: block;
	width: 100%;
	max-width: 275px;
	height: 380px;
	margin: auto;
	padding: 1.3rem;
	border: 2px solid rgb(246, 247, 248);
}
</style>
