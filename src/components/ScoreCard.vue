<template>
	<div class="flex flex-col gap-4 items-center p-4 bg-white text-slate-600 rounded-xl shadow-md">
		<section>
			<h1 class="font-bold">Event Name</h1>
		</section>
		<section class="flex justify-center items-center gap-16 mx-12 my-6">
			<section class="flex flex-col items-center gap-4">
				<div class="font-bold flex items-center justify-center bg-slate-200 rounded-full w-24 h-24"><h1 class="bg-white rounded-full shadow-md w-16 h-16 flex items-center justify-center">{{ t1 }}</h1></div>
				<h2>{{ t1 }}</h2>
			</section>
			<section class="flex gap-2 text-4xl">
				<h2 class="font-bold">3</h2>
				<span>:</span>
				<h2 class="font-bold">2</h2>
			</section>
			<section class="flex flex-col items-center gap-4">
				<div class="font-bold flex items-center justify-center bg-slate-200 rounded-full w-24 h-24"><h1 class="bg-white rounded-full shadow-md w-16 h-16 flex items-center justify-center">{{ t2 }}</h1></div>
				<h2>{{ t2 }}</h2>
			</section>
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