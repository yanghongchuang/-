<template>
	<div class="head">
		<div class="img">
			<img :src="item.bigImg" alt="">
			<h2>{{item.name}}</h2>
		</div>
		<div class="inc">
			<div class="top cf">
				<div class="left">
					<span class="score">{{item.score}}</span>
					<span>分</span>
					<span class="big">{{item.scorename}}</span>
					<div>{{item.commitCount}}条评论</div>
					<em class="iconfont">&#xe624;</em>
				</div>
				<div class="right">
					<div>景点简介</div>
					<div class="ziti">开放时间、贴士</div>
					<em class="iconfont">&#xe624;</em>
				</div>
			</div>
			<div class="but"><span class="iconfont">&#xe640;</span>{{item.address}}<em class="iconfont">&#xe624;</em></div>
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
	img{
		display: block;
		width: 100%;
	}
	.img{
		position: relative;
	}
	h2{
		font-size: 0.18rem;
		color: #fff;
		text-shadow: 0 1px 2px rgba(0,0,0,0.70);
		position: absolute;
		bottom: 15px;
		left: 0;
		padding-left: 10px;
		font-weight: normal;
		width: 100%;
		text-align: left;
	}
	h2:after{
		content: " ";
	    display: block;
	    position: absolute;
	    bottom: -14px;
	    left: 0;
	    width: 100%;
	    min-height: .3rem;
	    background-image: linear-gradient(to bottom,rgba(0,0,0,0),rgba(0,0,0,.8));
	}
	.inc{
		position: relative;
		top: -0.05rem;
		padding: 0.05rem 0.1rem 0 0.1rem;
		margin-bottom: 0.05rem;
		border-radius: 0.05rem 0.05rem 0 0;
		background: #fff;
		font-size: 0.12rem;
	}
	.top{
		padding-top: 0.05rem;
		padding-bottom: 0.1rem;
		border-bottom: 1px solid #e9e9e9;
	}
	.left{
		position: relative;
		border-right: 1px solid #e9e9e9;
		box-sizing: border-box;
		float: left;
		width: 50%;
	}
	.left .big{
		font-size: 0.14rem;
		display: inline-block;
		margin-left: 5px;
	}
	.left span{
		color: #ff8300;
	}
	.left .score{
		font-size: 0.22rem;
		line-height: 0.22rem;
	}
	.left div{
		color: #9e9e9e;
	}
	.right{
		position: relative;
		float: left;
		width: 50%;
	}
	.right div{
		padding-left: 0.15rem;
		font-size: 0.14rem;
		color: #212121;
	}
	.right .ziti{
		color: #9e9e9e;
		font-size: 0.12rem;
	}
	.but{
		color: #212121;
		font-size: 0.14rem;
		padding: 10px 0;
		line-height: 0.18rem;
		position: relative;
	}
	.but em{
		top: 25%;
	}
	.but span{
		display: inline-block;
		margin-right: 5px;
	}
	em{
		position: absolute;
		right: 10px;
		top: 40%;
		font-size: 0.12rem;
		transform: rotate(180deg);
	}
</style>