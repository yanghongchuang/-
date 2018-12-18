<template>
	<div class="w">
		<div>
			<a href="#">
				<img src="@/assets/images/1.png" alt="">
				<p>景点门票</p>
			</a>
			<a href="#">
				<img src="http://img1.qunarzz.com/piao/fusion/1811/f6/e54fad3ea337b02.gif" alt="">
				<p>立减30</p>
			</a>
			<a href="#">
				<img src="@/assets/images/3.png" alt="">
				<p>游乐场</p>
			</a>
			<a href="#">
				<img src="@/assets/images/4.png" alt="">
				<p>咸阳必游</p>
			</a>
			<a href="#">
				<img src="@/assets/images/5.png" alt="">
				<p>全部玩乐</p>
			</a>
		</div>
		<ul>
			<li class="li1"><span class="iconfont">&#xe640;</span>定位失败</li>
			<li><span class="iconfont">&#xe642;</span>必游榜单</li>
		</ul>
		<ol>
			<li  class="li1">
				<img src="@/assets/images/999862443f79a902.png" alt="">
			</li>
			<li>
				<img src="@/assets/images/f76d565689d9a202.png" alt="">
			</li>
		</ol>
	</div>
</template>
<script>
  export default {
    data() {
      return {
      }
    },
  }
</script>
<style scoped>
	ul,.w>div{
		overflow: hidden;
		border-top: 1px solid #eee;
		background: #fff;
	}
	.w>div{
		padding-bottom: 0.2rem;
	}
	ul{
		margin-bottom: 0.1rem;
	}
	ul li{
		line-height: 0.49rem;
		width: 50%;
		height: 0.49rem;
		float: left;
		font-size: 0.14rem;
		box-sizing: border-box;
	}
	ul li span{
		display: inline-block;
		margin-right: 3px;
	}
	.li1{
		border-right: 1px solid #eee;
	}
	ol{
		margin-bottom: .1rem;
		overflow: hidden;
		background: #fff;
		height: 0.7rem;
		text-align: left;
	}
	ol li{
		padding: 0 0.1rem;
		height: 100%;
		width: 50%;
		float: left;
		box-sizing: border-box;
	}
	ol li img{
		width: 100%;
	}
	ul li{
		text-align: center;
	}
	ol img{
		width: 100%;
	}
</style>