<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import SideBar from './components/SideBar.vue';
import MatchHistory from './components/MatchHistory.vue';
import NavBar from './components/NavBar.vue';
import Scores from './components/Scores.vue';
</script>

<template>
	<SideBar />
	<div class="flex flex-col w-full scores">
		<NavBar />
		<div class="flex">
			<MatchHistory />
			<Scores />
		</div>
	</div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');

body {
	overflow: hidden;
}

#app {
	font-family: 'Montserrat', sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	color: black;
	display: flex;
}

.scores {
	max-width: calc(100vw - 62.775px);
}
</style>
