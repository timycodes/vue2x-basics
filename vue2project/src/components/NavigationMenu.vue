<template>
	<div class="nav-container">
		<div class="nav">
			<nav :style="{ background: background || '#fff' }" class="nav-links">
				<ul>
					<router-link class="rlink" to="/">Home</router-link>
					|
					<router-link class="rlink" to="/about">About</router-link>
					|
					<router-link class="rlink" to="/portfolio">Portfolio</router-link>
					|
					<router-link class="rlink" to="/contact">Contact</router-link>
				</ul>
			</nav>
		</div>
	</div>
</template>

<script>
export default {
	name: 'NavigationMenu',
};
</script>

<style scoped lang="scss">
@import 'https://unpkg.com/ionicons@4.2.2/dist/css/ionicons.min.css';

.nav-links {
	display: flex;
	justify-content: space-around;
	align-content: center;
	height: 60px;
}
ul {
	margin: 0.2rem;
}
.rlink {
	display: inline-block;
	background: rgb(180, 180, 161);
	text-decoration: none;
	padding: 1rem;
	margin: 0;
	border: 1px solid black;
	border-radius: 5rem;
}
</style>
