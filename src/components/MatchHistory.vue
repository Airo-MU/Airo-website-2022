<script setup>
import MiniScoreCard from './MiniScoreCard.vue';
</script>

<template>
	<div class="flex flex-col gap-10 h-screen p-8 border-r-2 border-slate-200 overflow-y-scroll">
		<section class="flex flex-col gap-6">
			<h1 class="font-bold">Recent Match</h1>
			<div class="flex flex-col gap-4 items-center p-4 border-2 bg-slate-100 border-slate-200 text-slate-600 rounded-xl">
				<section class="flex items-center gap-4">
					<div class="font-bold flex items-center justify-center bg-slate-200 rounded-full w-16 h-16">MU</div>
					<h2>vs</h2>
					<div class="font-bold flex items-center justify-center bg-slate-200 rounded-full w-16 h-16">BITS</div>
				</section>
				<section class="flex gap-2">
					<h2 class="font-bold">3</h2>
					<span>:</span>
					<h2 class="font-bold">2</h2>
				</section>
			</div>
		</section>
		<section class="flex flex-col gap-6">
			<h1 class="font-bold">Previous Matches</h1>
			<mini-score-card t1="BITS" t2="JNTU" />
			<mini-score-card t1="X1" t2="X2" />
			<mini-score-card t1="X4" t2="X3" />
			<mini-score-card t1="X2" t2="JNTU" />
		</section>
	</div>
</template>

<style>
::-webkit-scrollbar {
	width: 0px;
	background: transparent;
}
</style>