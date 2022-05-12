<template>
	<nav class="fixed z-50 flex flex-col gap-8 h-screen p-4 border-r-2 bg-white border-slate-200 overflow-hidden" :class="{'w-side': expand, 'w-16': !expand}">
		<button class="ml-1" @click="expand = !expand">
			<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
				<path d="M21 15.61L19.59 17L14.58 12L19.59 7L21 8.39L17.44 12L21 15.61ZM3 6H16V8H3V6ZM3 13V11H13V13H3ZM3 18V16H16V18H3Z" fill="black"/>
			</svg>
		</button>
		<ul class="ml-1 flex gap-6 flex-col text-slate-500">
			<li><a href="" class="flex gap-6 items-center"><img src="../assets/Football.svg"> <h2>Cricket</h2></a></li>
			<li><a href="" class="flex gap-6 items-center"><img src="../assets/Football.svg"> <h2>Basketball</h2></a></li>
			<li><a href="" class="flex gap-6 items-center"><img src="../assets/Football.svg"> <h2>Badminton</h2></a></li>
			<li><a href="" class="flex gap-6 items-center"><img src="../assets/Football.svg"> <h2>Football</h2></a></li>
			<li><a href="" class="flex gap-6 items-center"><img src="../assets/Football.svg"> <h2>Volleyball</h2></a></li>
			<li><a href="" class="flex gap-6 items-center"><img src="../assets/Football.svg"> <h2>Throwball</h2></a></li>
			<li><a href="" class="flex gap-6 items-center"><img src="../assets/Football.svg"> <h2>Chess</h2></a></li>
			<li><a href="" class="flex gap-6 items-center"><img src="../assets/Football.svg"> <h2>TT</h2></a></li>
			<li><a href="" class="flex gap-6 items-center"><img src="../assets/Football.svg"> <h2>Pool</h2></a></li>
			<li><a href="" class="flex gap-6 items-center"><img src="../assets/Football.svg"> <h2>Snooker</h2></a></li>
			<li><a href="" class="flex gap-6 items-center"><img src="../assets/Football.svg"> <h2>KhoKho</h2></a></li>
			<li><a href="" class="flex gap-6 items-center"><img src="../assets/Football.svg"> <h2>Tennis</h2></a></li>
		</ul>
	</nav>

	<div class="fixed z-40 w-screen h-screen bg-white/40 backdrop-blur-sm" v-if="expand" @click="expand = !expand"></div>
</template>

<script>
export default {
	data() {
		return {
			expand: false
		}
	}
}
</script>

<style>
.w-side {
	width: 260px;
}
</style>
