<template>
	<div id="app">
		<div class="girl-container">
			<img class="face" alt="artwork of female face" src="./assets/girl.jpg" />
		</div>
		<HelloWorld msg="Tim Conroy | Frontend Developer" />
	</div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
	name: 'App',
	components: {
		HelloWorld,
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
