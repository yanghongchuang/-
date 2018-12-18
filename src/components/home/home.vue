<template>
	<div>
		<head-swiper></head-swiper>
		<lunbo-swiper></lunbo-swiper>
		<icon-swiper></icon-swiper>
		<bangdan-swiper></bangdan-swiper>
		<liebiao-swiper></liebiao-swiper>
		<weekend-swiper></weekend-swiper>
	</div>
</template>
<script>
	import lunboSwiper from "./module/swiper"
	import headSwiper from "./module/head"
	import iconSwiper from "./module/icon"
	import bangdanSwiper from "./module/bangdan"
	import liebiaoSwiper from "./module/liebiao"
	import weekendSwiper from "./module/weekend"
	export default {
		data() {
			return {}
		},
		components:{
			lunboSwiper,
			headSwiper,
			iconSwiper,
			bangdanSwiper,
			liebiaoSwiper,
			weekendSwiper
		}
	}
</script>
