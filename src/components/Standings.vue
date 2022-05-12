<template>
	<div class="flex flex-col gap-6 h-scores p-6 lg:p-8 border-r-2 border-slate-200">
		<h1 class="font-bold">Standings</h1>
		<section>
			<section class="flex flex-col w-matches">
				<div class="grid gap-4 grid-cols-2 bg-slate-200 text-slate-600 px-4 py-3 border-x-2 border-t-2 border-slate-200 rounded-t-xl text-lg">
					<div class="font-bold">Team</div>
					<div class="font-bold">Item</div>
				</div>
			</section>
			<div class="flex flex-col border-2 border-slate-200 rounded-b-xl divide-y-2 divide-dashed w-matches h-matches overflow-y-scroll">
				<section v-for="i in 17" :key="i">
					<div class="grid gap-4 grid-cols-2 text-slate-600 px-4 py-2">
						<div class="font-bold">Team {{ i }}</div>
						<div>{{ i + 3 }}</div>
					</div>
				</section>
			</div>
		</section>
	</div>
</template>

<style>
.standings {
	min-width: 360px;
}

@media (max-width: 1024px) {
	.w-matches {
		width: auto;
	}
}
</style>