<template>
	<div class="flex flex-col gap-10 h-screen w-full standings px-12 py-8 border-r-2 border-slate-200">
		<h1 class="font-bold">Standings</h1>
		<section class="border-2 border-slate-200 rounded-lg p-8 overflow-y-scroll mb-16">
			<div class="flex flex-col gap-6">
				<div class="flex justify-between font-bold">
					<span>Team</span>
					<span>Info</span>
				</div>
				<div v-for="i in 15" :key="i" class="flex justify-between">
					<span>Team {{i}}</span>
					<span>X{{i}}</span>
				</div>
			</div>
		</section>
	</div>
</template>

<style>
.standings {
	min-width: 360px;
}
</style>