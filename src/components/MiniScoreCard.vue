<template>
	<div class="flex flex-col gap-4 items-center px-8 py-4 border-2 border-slate-200 text-slate-600 rounded-xl">
		<section class="flex items-center gap-6">
			<div class="font-bold flex items-center justify-center bg-slate-200 rounded-full w-16 h-16">{{ t1 }}</div>
			<h2>vs</h2>
			<div class="font-bold flex items-center justify-center bg-slate-200 rounded-full w-16 h-16">{{ t2 }}</div>
		</section>
		<section class="flex gap-2">
			<h2 class="font-bold">3</h2>
			<span>:</span>
			<h2 class="font-bold">2</h2>
		</section>
	</div>
</template>

<script>
export default {
	props: {
		t1: String,
		t2: String
	}
}
</script>