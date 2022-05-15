<template>
	<div class="flex flex-col h-scores p-6 lg:p-8 border-r-2 border-slate-200">
		<section class="flex flex-col w-matches gap-6">
			<h1 class="font-bold">{{ event }} Matches</h1>
			<div class="grid gap-4 grid-cols-3 justify-items-center bg-slate-200 text-slate-600 py-3 border-x-2 border-t-2 border-slate-200 rounded-t-xl text-lg">
				<div class="font-bold">X</div>
				<section class="flex gap-2">
					<span>vs</span>
				</section>
				<div class="font-bold">Y</div>
			</div>
		</section>
		<div class="flex flex-col border-2 border-slate-200 rounded-b-xl divide-y-2 divide-dashed w-matches h-matches overflow-y-scroll">
			<section v-for="i in cricket" :key="i">
				<div class="grid gap-4 grid-cols-3 justify-items-center text-slate-600 py-2">
					<div class="font-bold">{{ i.bat_team }}</div>
					<section class="flex gap-2">
						<h2>{{ i.runs }}</h2>
						<span>/</span>
						<h2>{{ i.wickets }}</h2>
					</section>
					<div class="font-bold">{{ i.bowl_team }}</div>
				</div>
			</section>
		</div>
	</div>
</template>

<script>
import axios from "axios"

export default {
	data() {
		return {
			cricket: []
		}
	},
	props: {
		event: String
	},
	created() {
		axios
			.get("https://raw.githubusercontent.com/Airo-MU/matches/master/cricket/cricket.json")
			.then((res) => {
				this.cricket = res.data
			})
	}
}
</script>

<style>
::-webkit-scrollbar {
	width: 0px;
	background: transparent;
}

.w-matches {
	width: 320px;
}

.h-matches {
	max-height: 506px;
}
</style>