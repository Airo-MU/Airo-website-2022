<template>
	<nav class="flex flex-col gap-8 h-screen p-4 border-r-2 border-slate-200 transition-transform ease-in-out duration-200 overflow-hidden" :class="{'w-full bg-slate-100': expand, 'w-16': !expand}">
		<button class="ml-1" @click="expand = !expand">
			<svg width="25" height="25" viewBox="0 0 25 25" fill="none" xmlns="http://www.w3.org/2000/svg">
				<path d="M3.00781 6.03906H21.0078V8.03906H3.00781V6.03906ZM3.00781 11.0391H21.0078V13.0391H3.00781V11.0391ZM3.00781 16.0391H21.0078V18.0391H3.00781V16.0391Z" fill="black"/>
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
