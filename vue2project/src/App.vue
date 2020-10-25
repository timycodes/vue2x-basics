<template>
	<div id="app">
		<NavigationMenu></NavigationMenu>
		<div class="girl-container">
			<img class="face" alt="artwork of female face" src="./assets/girl.jpg" />
		</div>
		<img class="vuelogo" alt="vue logo" src="./assets/logo.png" />

		<MyProfile msg="Tim Conroy | Frontend Developer" />
	</div>
</template>

<script>
import MyProfile from './components/MyProfile';
import NavigationMenu from './components/NavigationMenu';

export default {
	name: 'App',
	components: {
		MyProfile,
		NavigationMenu,
	},
};
</script>

<style>
#app {
	font-family: 'Roboto', sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}

.girl-container {
	display: flex;
	align-items: center;
	justify-content: center;
	border: 2px solid black;
	margin: auto;
	background-color: black;
}
.face {
	display: block;
	width: 100%;
	max-width: 275px;
	height: 380px;
	margin: auto;
	padding: 1.3rem;
	border: 2px solid white;
}
</style>
