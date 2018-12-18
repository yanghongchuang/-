<template>
	<div>
		<h2>
			<div class="fl">
				<img src="@/assets/images/ico.png" alt="">
				本周热门榜单
			</div>
			<a class="fr">
				全部榜单
				<span class="iconfont">&#xe624;</span>
			</a>
		</h2>
		<div class="w">
			<ul>
				<li v-for="item of liList">
					<img :src="item.src1" class="abs">
					<img :src="item.src">
					<p>{{item.title}}</p>
					<div><span>{{item.price}}</span>起</div>
				</li>
			</ul>
		</div>
	</div>
</template>
<script>
	export default {
		data(){
			return{
				liList:[
					{
						id:0,
						src:"http://img1.qunarzz.com/sight/p0/1505/2e/2eb25cce70d82954.water.jpg_250x250_4f1ff835.jpg",
						title:"乾陵",
						price:"￥70",
						src1:"http://img1.qunarzz.com/piao/fusion/1710/ab/159673b63e6ca702.png"
					},
					{
						id:1,
						src:"http://img1.qunarzz.com/sight/p0/1505/31/31008ea4c8ebd546.water.jpg_250x250_a2feac59.jpg",
						title:"汉阳陵博物馆",
						price:"￥50",
						src1:"http://img1.qunarzz.com/piao/fusion/1710/2d/36d0c4adaebbbc02.png"
					},
					{
						id:2,
						src:"http://img1.qunarzz.com/sight/p0/201301/05/129b8cd36466c12e93835fbb.png_250x250_585f0aa8.png",
						title:"西北农林科技大学",
						price:"￥27",
						src1:"http://img1.qunarzz.com/piao/fusion/1710/67/edc47ffef9e96b02.png"
					},
					{
						id:3,
						src:"http://img1.qunarzz.com/sight/p0/1411/9d/d74294e6031d93218b9ccfa621926d25.water.jpg_250x250_e993bb61.jpg",
						title:"咸阳海泉湾温泉",
						price:"￥148"
					},
					{
						id:4,
						src:"http://img1.qunarzz.com/sight/p0/1505/b0/b093339694db4a11.water.jpg_250x250_7b1cfb31.jpg",
						title:"张裕瑞纳城堡酒庄",
						price:"￥96"
					},
					{
						id:5,
						src:"http://img1.qunarzz.com/sight/p0/1411/5a/6dae7329dfb006893719e958f7e274a9.water.jpg_250x250_3e8a810c.jpg",
						title:"茂林博物馆",
						price:"￥50"
					},
					{
						id:6,
						src:"http://img1.qunarzz.com/sight/p0/1606/d2/d25becf22ed8c26ee2.water.jpg_250x250_05b51a50.jpg",
						title:"蓝波湾温泉水世界",
						price:"￥68"
					},
					{
						id:7,
						src:"http://img1.qunarzz.com/sight/p0/1805/93/93316ef975272467a3.img.png_250x250_c5d950e1.png",
						title:"跃趣蹦床运动工厂",
						price:"￥89"
					},
					{
						id:8,
						src:"http://img1.qunarzz.com/sight/p0/1707/85/8587a901385d27fca3.img.jpg_250x250_263690e2.jpg",
						title:"华韵温泉",
						price:"￥29.9"
					},
					{
						id:9,
						src:"http://img1.qunarzz.com/sight/p0/1807/46/469bff659a3f82cea3.img.jpg_250x250_dbc7c3f5.jpg",
						title:"姜嫄水乡",
						price:"￥8"
					},
				]
			}
		}
	}
</script>
<style scoped>
	div{
		background: #fff;
	}
	h2{
		padding: 0.12rem 0 0.13rem 0;
		font-size: 0.16rem;
		font-weight: normal;
		overflow: hidden;
	}
	.fl{
		float: left;
	}
	.fl img{
		display: inline-block;
		width: 0.15rem;
		height: 0.15rem;
		margin-left: 0.1rem;
		color: #212121;
		line-height: 0.22rem;
		vertical-align: top;
	}
	.fr{
		float: right;
		color: #616161;
		font-size: 0.12rem;
		position: relative;
		top: 4px;
	}
	.fr span{
		display: inline-block;
		font-size: 0.12rem;
		margin-right: 0.18rem;
		transform: rotate(180deg);
	}
	.w{
		overflow: hidden;
	    overflow-x: scroll;
	    white-space: nowrap;
	}
	ul{
		width: 1055px;
		padding: 0 12px;
	}
	ul li:last-child{
		margin-right: 0;
	}
	li{
		width: 1rem;
		height: 1.41rem;
		padding: 3px 0 10px 0;
		position: relative;
		float: left;
		font-size: 0.12rem;
		color: #212121;
		text-align: center;
		margin-right: 6px;
	}
	li img{
		height: 1rem;
	}
	li p{
		margin-top: 6px;
	}
	li span{
		color:#ff8300;
	}
	li div{
		color: #616161;
	}
	.abs{
		height: 20px;
		position: absolute;
		top: 0;
		left: 0;
	}
</style>