<template>
	<div>
		<list :item="product"></list>
		<advice :item="product"></advice>
		<promotion :item="product"></promotion>
		<ticket :item="product"></ticket>
		<taopiao :item="product"></taopiao>
		<coment :item="product"></coment>
	</div>
</template>
<script>
	import axios from "axios"
	import list from "./module/list"
	import advice from "./module/advice"
	import promotion from "./module/promotion"
	import ticket from "./module/ticket"
	import taopiao from "./module/taopiao"
	import coment from "./module/coment"
	export default {
		data(){
			return{
				product:{
					address: null,
					bigImg: null,
					comment: null,
					commitCount: null,
					id: null,
					name: null,
					product: {},
					score: null,
					scorename: null,
					strategy: null
				}
			}
		},
		components:{
			list,
			advice,
			promotion,
			ticket,
			taopiao,
			coment
		},
		mounted(){
			axios.get("http://192.168.1.104:8080/static/mock/qunar.json").then((response)=>{
				this.product = response.data[this.$route.params.id]
				console.log(this.product)
			})
		}
	}
</script>