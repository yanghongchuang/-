<template>
	<div class="pro">
		<h2>用户评价</h2>
		<div class="pad"  v-for="ite of item.product.comment">
			<div class="top cf">
				<div class="left">
					<span class="score1" :style="{width:item.score}">★★★★★</span>
					<span class="score">★★★★★</span>
				</div>
				<div class="right">
					<span>{{ite.username}}</span>
					<span>{{ite.time}}</span>
				</div>
			</div>
			<div class="but"></div>
		</div>
	</div>
</template>
<script>
	export default {
		data(){
			return{

			}
		},
		props:["item"]
	}
</script>
<style scoped>
	.pro{
		margin-top: 10px;
		background: #fff;
		font-size: 0.14rem;
	}
	h2{
		text-indent: 0.18rem;
		font-size: 0.16rem;
		font-weight: normal;
		color: #333;
		line-height: 0.44rem;
		height: 0.44rem;
		border-bottom: 1px solid #eee;
		position: relative;
		padding-left: 3px;
		position: relative;
	}
	h2:after{
		content: " ";
	    position: absolute;
	    top: .16rem;
	    left: .1rem;
	    width: .03rem;
	    height: .13rem;
	    background: #1ba9ba;
        border-radius: .02rem;
	}
	.pad{
		padding: 5px 10px 15px 10px;
	}
	.left{
		float: left;
		position: relative;
		letter-spacing: 0.5px;
		width: 51px;
		height: 14px;
	}
	.score{
		display: inline-block;
		color: #e0e0e0;
		z-index: 1;
	}
	.score1{
		color: #ffb436;
		z-index: 2;
		overflow: hidden;
	}
	.left span{
		position: absolute;
	}
	.right{
		float: right;
	}
	.top{
		margin-top: 10px;
	}
</style>