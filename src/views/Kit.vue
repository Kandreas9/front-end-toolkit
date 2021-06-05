<template>
	<div
		class="content-circle html"
		:class="[isHtmlActive ? 'active' : 'html']"
		@click="isHtmlActive = !isHtmlActive"
	></div>
	<div
		class="content-circle"
		:class="[isCssActive ? 'active' : 'css']"
		@click="isCssActive = !isCssActive"
	></div>
	<div
		class="content-circle"
		:class="[isJsActive ? 'active' : 'js']"
		@click="isJsActive = !isJsActive"
	></div>
</template>

<script>
export default {
	name: "Kit",
	data() {
		return {
			isHtmlActive: false,
			isCssActive: false,
			isJsActive: false,
		};
	},
};
</script>

<style>
.content-circle {
	background-color: var(--primary-color);
	border-radius: 50%;
	box-shadow: 6px 6px 4px rgba(0, 0, 0, 0.25);
	transform: scale(1);
	transition: 1.5s;
}

.html {
	position: absolute;
	height: 100px;
	width: 100px;
	top: 100px;
	left: 100px;
}

.css {
	position: absolute;
	height: 170px;
	width: 170px;
	top: 280px;
	right: 70px;
}

.js {
	position: absolute;
	height: 130px;
	width: 130px;
}

.active {
	position: absolute;
	top: 43%;
	left: 40%;
	z-index: 10;
	transform: translate(-50%, -50%);
	transform: scale(7);
}
</style>
