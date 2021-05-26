<template>
	<header class="home">
		<h1 class="home-title">Front-End Starter Kit</h1>
		<router-link class="home-btn" to="/about">Get Started</router-link>
	</header>
</template>

<script>
export default {
	name: "Home",
};
</script>

<style>
.home {
	display: flex;
	flex-direction: column;
	align-items: center;
	font-size: 1.3rem;
}

.home-title {
	max-width: 8ch;
	margin-bottom: 1.5rem;
	text-align: center;
	font-weight: bold;
	font-size: 4rem;
	color: var(--secondary-color);
	text-shadow: 1px 1px var(--secondary-color-light),
		2px 2px var(--secondary-color-light),
		3px 3px var(--secondary-color-light),
		4px 4px var(--secondary-color-light),
		5px 5px var(--secondary-color-light),
		6px 6px var(--secondary-color-light);
}

.home-btn {
	width: 10rem;
	text-align: center;
	color: var(--secondary-color);
	text-decoration: none;
	padding: 0.5rem 0.9rem;
	background: var(--primary-color);
	box-shadow: 6px 6px 4px rgba(0, 0, 0, 0.25);
	border-radius: 27px;
}

.home-btn:hover {
	font-weight: bold;
	background: #ac4590;
}
</style>
