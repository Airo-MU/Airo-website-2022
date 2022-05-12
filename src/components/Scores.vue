<script setup>
import ScoreCard from './ScoreCard.vue';
</script>

<template>
	<div class="flex flex-col gap-6 lg:gap-12 h-scores w-sc lg:w-full px-6 lg:px-12 py-6 bg-slate-50 border-r-2 border-slate-200 overflow-y-scroll">
		<div class="flex flex-col gap-3 lg:gap-6">
			<h1 class="font-bold text-slate-500">Recent</h1>
			<ScoreCard t1="MU" t2="BITS" />
		</div>
		<div class="flex flex-col gap-3 lg:gap-6">
			<h1 class="font-bold text-slate-500">Last Match</h1>
			<ScoreCard t1="BITS" t2="JNTU" />
		</div>
	</div>
</template>

<style>
::-webkit-scrollbar {
	width: 0px;
	background: transparent;
}
</style>