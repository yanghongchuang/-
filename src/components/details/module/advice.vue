<template>
	<div class="adv">
		<div class="where">
			<h2>去哪儿推荐</h2>
			<div v-for="ite of item.product.recommend" class="list cf">
				<div class="left">
					<p>{{ite.name}}</p>
					<div class="yuding">{{ite.remark}}</div>
					<div class="gift">
						<span v-if="ite.label[0]">{{ite.label[0]}}</span>
						<span v-if="ite.label[1]">{{ite.label[1]}}</span>
						<span class="red" v-if="ite.label[2]">{{ite.label[2]}}</span>
					</div>
				</div>
				<div class="right">
					<div class="pri">￥<span>{{ite.price}}</span></div>
					<div class="anniu">预定</div>
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
	.adv{
		margin-top: 10px;
		background: #fff;
		font-size: 0.14rem;
	}
	.where{
		padding-left: 10px;
		margin-bottom: 10px;
	}
	h2{
		background: url('../../../assets/images/zan.png') no-repeat 0 center;
		background-size: .18rem .18rem;
		text-indent: 0.18rem;
		font-size: 0.16rem;
		font-weight: normal;
		color: #333;
		line-height: 0.44rem;
		height: 0.44rem;
		padding: 0 10px;
		border-bottom: 1px solid #eee;
	}
	.list{
		font-size: 0.14rem;
		color:#616161;
		padding: 10px 10px 12px 0;
	}
	.left{
		float: left;
		width: 70%;
		font-size: 0.15rem;
		margin-right: 0.05rem;
		line-height: 0.26rem;
		display: -webkit-box;
	    overflow: hidden;
	    text-overflow: ellipsis;
	    -webkit-line-clamp: 2;
	    -webkit-box-orient: vertical;
	}
	.yuding{
		height: .16rem;
		font-size: .12rem;
		line-height: .16rem;
		white-space: nowrap;
	}
	.gift span{
		display: inline-block;
	    margin-top: .04rem;
	    padding: 0 .02rem;
	    height: .16rem;
	    color: #00afc7;
	    font-size: .1rem;
	    line-height: .16rem;
	    white-space: nowrap;
	    border-radius: 4px;
	   	border: 1px solid #a5e4ec;
	}
	.pri{
		color: #ff9800;
	}
	.pri span{
		margin-left: .02rem;
	    font-size: .2rem;
	    line-height: .2rem;
	}
	.right{
		margin-top: 15px;
		text-align: center;
		float: right;
	}
	.anniu{
		border-radius: 0.04rem;
		width: 0.8rem;
		height: .3rem;
	    color: #fff;
	    font-size: .14rem;
	    line-height: .3rem;
	    background-image: linear-gradient(130deg,#ffab1e 37%,#ff8c12 100%);
	}
</style>