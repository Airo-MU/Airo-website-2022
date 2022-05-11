<template>
	<header class="flex p-4 border-b-2 border-slate-200 overflow-y-scroll">
		<nav>
			<ul class="flex gap-6">
				<li>Live Stream</li>
				<li v-for="i in 2" :key="i">Item {{ i }}</li>
			</ul>
		</nav>
	</header>
</template>