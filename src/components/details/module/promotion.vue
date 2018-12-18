<template>
	<div class="pro">
		<div class="ticket">
			<h2><span></span>促销</h2>
			<div class="con cf" v-for="ite of item.product.sale">
				<div class="left">
					<p>{{ite.name}}</p>
				</div>
				<div class="right">
					<span class="pir">￥<span>{{ite.price}}</span></span>
					起<em class="iconfont">&#xe62f;</em>
				</div>
			</div>
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
	.ticket{
		padding-left: 10px;
		margin-bottom: 10px;
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
	}
	h2 span{
		position: absolute;
		left: 0;
		top: 0.13rem;
		display: inline-block;
		background-size: 20px !important;
		width: .18rem;
		height: .18rem;
		background: url('../../../assets/images/detail.png') no-repeat 0 -.22rem;
	}
	.con{
		padding: 12px 10px;
	}
	.left{
		float: left;
		width: 70%;
		font-size: 0.15rem;
		color: #333;
		line-height: 0.24rem;
	}
	.pir{
		color: #ff9800;
	}
	.right{
		text-align: center;
		float: right;
		color: #9e9e9e;
		font-size: 0.12rem;
	}
	.right span{
		margin-left: .02rem;
	    font-size: .2rem;
	    line-height: .2rem;
	}
	em{
		font-size: 0.14rem;
	}
</style>