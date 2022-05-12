<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import SideBar from './components/SideBar.vue';
import MatchHistory from './components/MatchHistory.vue';
import NavBar from './components/NavBar.vue';
import Scores from './components/Scores.vue';
import Standings from './components/Standings.vue';
</script>

<template>
	<SideBar />
	<NavBar />
	<div class="flex flex-col lg:flex-row scores overflow-y-scroll">
		<MatchHistory class="hidden xl:block" />
		<Scores />
		<Standings />
		<MatchHistory class="md:hidden block" />
	</div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');

#app {
	font-family: 'Montserrat', sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	color: black;
	display: flex;
	flex-direction: column;
}

.scores {
	max-width: calc(100vw - 62px);
	margin-left: 62px;
}

.h-scores {
	height: calc(100vh - 58px);
}

@media (max-width: 1024px) {
	.scores {
		width: calc(100vw - 62px);
	}

	.h-scores {
		height: auto;
	}

	.w-sc {
		max-width: calc(100vw - 62px);
	}
}
</style>
