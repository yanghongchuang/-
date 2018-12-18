<template>
	<header>
		<i class="iconfont">&#xe624;</i>
		<div class="search">
			<b class="iconfont">&#xe635;</b>
			<input type="text" placeholder="输入城市/景点/游玩主题">
		</div>
		<span>{{city}}<em class="iconfont">&#xe62f;</em></span>
	</header>
</template>
<script>
  export default {
    data() {
      return {
      	city:"咸阳"
      }
    },
  }
</script>
<style>
 	img{
 		display: block;
 	}
	header{
		height: 0.44rem;
		line-height: 0.44rem;
		background-color: #00bcd4;
		font-size: 0.14rem;
		overflow: hidden;
		color: #fff;
	}
	header i{
		float: left;
		width: 15%;
	}
	header .search{
		float: left;
		width: 68%;
	}
	.search{
		position: relative;
	}
	.search b{
		color: #e3e3e3;
		position: absolute;
		left: 7px;
		font-style: normal;
	}
	.search input{
		text-indent: 0.3rem;
		width: 100%;
		border: 0;
		height: 0.3rem;
		border-radius: 4px;
	}
	input::-webkit-input-placeholder{
		color: #e3e3e3;
	}
	header span{
		float: right;
		width: 15%;
	}
	span em{
		position: relative;
		top: 2px;
		left: 2px;
	}
	.w a{
		text-decoration: none;
		display: block;
		float: left;
		width: 25%;
		height: 0.8rem;
		padding-top: 5px;
		text-align: center;
	}
	.w>div{
		padding-top: 0.1rem;
	}
	a img{
		margin:0 auto ;
		display: block;
		width: 0.55rem;
		height: 0.55rem;
	}
	a p{
		margin-top: 0.05rem;
		color: #212121;
		font-size: .14rem;
	}
	.swiper-pagination-bullet{
		width: 6px !important;
		height: 6px !important;
	}
	.swiper-pagination-bullet-active{
		background-color: #fff !important;
	}
	.swiper-container-horizontal>.swiper-pagination-bullets,
	.swiper-pagination-custom,
	.swiper-pagination-fraction {
    bottom: -15px !important;
    left: 0 !important;
    width: 100% !important;
}
</style>