<template>
	<div class="w2">
		<h2>
			<div class="fl">
				<img src="@/assets/images/icon2.png" alt="">
				猜你喜欢
			</div>
		</h2>
		<ul>
			<router-link tag="li" :to="/details/+ item.id" v-for="item of liList" :key="item.id">
				<a href="" class="cf">
					<div class="left">
						<img :src="item.src">
						<div class="abs" v-if="item.title"><span>{{item.title}}</span></div>
					</div>
					<div class="right">
						<div class="biaoti">{{item.biaoti}}</div>
						<div class="pinlun">
							<span class="span">
								<span class="score1" :style="{width:item.score}">★★★★★</span>
								<span class="score">★★★★★</span>
							</span>
							<span class="com">{{item.pinlun}}</span>
						</div>
						<div class="price">
							<span>￥{{item.price}}</span>起
							<span class="adress">{{item.adress}}</span>
						</div>
						<div class="tishi">{{item.tishi}}</div>
					</div>
				</a>
			</router-link>
		</ul>
		<a href="" class="search">查看所有产品</a>
	</div>
</template>
<script>
  export default {
    data() {
    	return{
    		liList:[
    			{
    				id:10,
    				src:"http://img1.qunarzz.com/sight/p0/1505/b0/b093339694db4a11.water.jpg_200x200_10f65a8e.jpg",
    				title:"可定明日",
    				biaoti:"张裕瑞那城堡酒庄",
    				pinlun:"1898条评论",
    				price:"96",
    				adress:"渭城区",
    				tishi:"近期小伙伴们收藏最！多！的景点😊",
    				score:"98%"
    			},
    			{
    				id:11,
    				src:"http://img1.qunarzz.com/sight/p0/1505/2e/2eb25cce70d82954.water.jpg_200x200_dd8cb4f2.jpg",
    				title:"可定明日",
    				biaoti:"乾陵",
    				pinlun:"3515条评论",
    				price:"70",
    				adress:"乾县",
    				tishi:"🔥好评如潮，小伙伴热推景点~",
    				score:"96%"
    			},
    			{
    				id:12,
    				src:"http://img1.qunarzz.com/sight/p0/1411/9d/d74294e6031d93218b9ccfa621926d25.water.jpg_200x200_bb991fa2.jpg",
    				biaoti:"咸阳海泉湾温泉世界",
    				pinlun:"813条评论",
    				price:"148",
    				adress:"秦都区",
    				score:"98%"
    			},
    			{
    				id:13,
    				src:"http://img1.qunarzz.com/sight/p0/1411/5a/6dae7329dfb006893719e958f7e274a9.water.jpg_200x200_2e291876.jpg",
    				title:"可定明日",
    				biaoti:"茂陵博物馆",
    				pinlun:"577条评论",
    				price:"50",
    				tishi:"👍小伙伴们都收藏了，去看看吧~",
    				score:"94%"
    			},
    			{
    				id:14,
    				src:"http://img1.qunarzz.com/sight/p0/1505/31/31008ea4c8ebd546.water.jpg_200x200_68c67c0b.jpg",
    				title:"随买随用",
    				biaoti:"汉阳陵博物馆",
    				pinlun:"1521条评论",
    				price:"50",
    				adress:"秦都区",
    				score:"96%"
    			},
    			{
    				id:15,
    				src:"http://img1.qunarzz.com/sight/p0/1606/d2/d25becf22ed8c26ee2.water.jpg_200x200_b726528e.jpg",
    				biaoti:"蓝波湾温泉水世界",
    				pinlun:"64条评论",
    				price:"68",
    				adress:"咸阳",
    				tishi:"咸阳本月收藏Top5╰(￣▽￣)╭",
    				score:"98%"
    			},
    			{
    				id:16,
    				src:"http://img1.qunarzz.com/sight/p0/1710/3b/3bd09821901efad5a3.img.jpg_200x200_1c934f6f.jpg",
    				biaoti:"侍郎湖",
    				pinlun:"64条评论",
    				price:"19.9",
    				adress:"彬县",
    				score:"98%"
    			},
    			{
    				id:17,
    				src:"http://img1.qunarzz.com/sight/p0/201304/09/3005b70fe5a65773c8d65eac.jpg_200x200_837f52ee.jpg",
    				biaoti:"郑国渠",
    				pinlun:"33条评论",
    				price:"45",
    				adress:"泾阳县",
    				score:"92%"
    			},
    			{
    				id:18,
    				src:"http://img1.qunarzz.com/sight/p0/201403/10/896a38118838b3d46a5a355020920a0d.jpg_200x200_dc0a367e.jpg",
    				biaoti:"咸阳湖景区",
    				pinlun:"115条评论",
    				price:"25",
    				adress:"秦都区",
    				score:"90%"
    			},
    			{
    				id:19,
    				src:"http://img1.qunarzz.com/sight/p0/201403/10/896a38118838b3d46a5a355020920a0d.jpg_200x200_dc0a367e.jpg",
    				title:"随买随用",
    				biaoti:"袁家村·关中大观园",
    				pinlun:"36条评论",
    				price:"20",
    				adress:"礼泉县",
    				score:"96%"
    			},
    			{
    				id:20,
    				src:"http://img1.qunarzz.com/sight/p0/1807/46/469bff659a3f82cea3.img.jpg_200x200_54795169.jpg",
    				biaoti:"姜嫄水乡",
    				pinlun:"2条评论",
    				price:"8",
    				adress:"咸阳",
    				score:"100%"
    			},
    			{
    				id:21,
    				src:"http://img1.qunarzz.com/sight/p0/1805/93/93316ef975272467a3.img.png_200x200_ae038519.png",
    				biaoti:"跃趣蹦床运动工厂",
    				pinlun:"53条评论",
    				price:"89",
    				adress:"秦都区",
    				score:"100%"
    			},
    			{
    				id:22,
    				src:"http://img1.qunarzz.com/sight/p0/1802/f8/f8e6406d05c03e08a3.water.jpg_200x200_aeb8ae49.jpg",
    				biaoti:"安吴堡",
    				pinlun:"1条评论",
    				price:"98",
    				adress:"泾阳县",
    				tishi:"流传了诸多极具传奇色彩的故事",
    				score:"60%"
    			},
    			{
    				id:23,
    				src:"http://img1.qunarzz.com/sight/p0/1703/57/5794796148ac680da3.img.png_200x200_0cf91d82.png",
    				biaoti:"乐华城•乐华欢乐世界",
    				pinlun:"6249条评论",
    				price:"200",
    				adress:"泾阳县",
    				score:"98%"
    			},
    			{
    				id:24,
    				src:"http://img1.qunarzz.com/sight/p0/201301/05/129b8cd36466c12e93835fbb.png_200x200_6f200759.png",
    				title:"可定明日",
    				biaoti:"西北农林科技大学博览园",
    				pinlun:"323条评论",
    				price:"27",
    				adress:"杨凌区",
    				tishi:"帅的人都去过了😎，你还等什么~",
    				score:"94%"
    			},
    			{
    				id:25,
    				src:"http://img1.qunarzz.com/sight/p0/201403/07/37d460397e3639447bcec4b747789763.jpg_200x200_4da983ee.jpg",
    				biaoti:"昭陵博物馆",
    				pinlun:"91条评论",
    				price:"25",
    				adress:"礼泉县",
    				tishi:"面积和陪葬墓之多居历代帝王陵墓之首",
    				score:"98%"
    			},
    			{
    				id:26,
    				src:"http://img1.qunarzz.com/sight/p0/1703/13/13f5ef4857706273a3.water.jpg_200x200_50ba2a87.jpg",
    				biaoti:"宏兴滑草滑雪体验基地",
    				pinlun:"",
    				price:"26",
    				adress:"兴平市",
    				score:"0%"
    			},
    			{
    				id:27,
    				src:"http://img1.qunarzz.com/sight/p0/1611/21/218bed923f3eda3ba3.water.jpg_200x200_a515d336.jpg",
    				biaoti:"唐昭陵",
    				pinlun:"86条评论",
    				price:"25",
    				adress:"礼泉县",
    				tishi:"古代帝王依山陵，唐代开放的缩影",
    				score:"100%"
    			},
    			{
    				id:28,
    				src:"http://img1.qunarzz.com/sight/p0/1707/85/8587a901385d27fca3.img.jpg_200x200_f7089b4f.jpg",
    				biaoti:"华韵温泉",
    				pinlun:"6条评论",
    				price:"29.9",
    				adress:"兴平市",
    				score:"90%"
    			}
    		]
    	}
    }
  }
</script>
<style scoped>
	.w2{
		margin-top: 0.1rem;
		background: #fff;
	}
	h2{
		padding: 0.12rem 0 0.13rem 0;
		font-size: 0.16rem;
		font-weight: normal;
		text-align: left;
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
	ul{
		margin-left: 0.12rem;
	}
	ul li{
		padding: 10px 0;
		border-bottom: 1px solid #ddd;
	}
	.left,.right{
		float: left;
	}
	.left img{
		height: 1rem;
		width: 1rem;
	}
	.left{
		position: relative;
	}
	.abs{
		background-image: url(https://img1.qunarzz.com/piao/fusion/1802/52/b9080e45b69b4f02.png);
		position: absolute;
		top: 0;
		left: 0;
		width: 0.51rem;
		height: 0.19rem;
		background-size: 100%;
		color: #fff;
		font-size: 0.12rem;
		line-height: 0.19rem;
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
	.span{
		letter-spacing: 0.5px;
		width: 51px;
		height: 14px;
		display: inline-block;
		position: relative;
	}
	.span span{
		position: absolute;
	}
	.com{
		margin-left: 10px;
	}
	.right{
		line-height: 0.2rem;
		width: 67%;
		padding-left: 11px;
		font-size: 0.12rem;
		text-align: left;
		color: #212121;
	}
	.right .biaoti{
		height: 0.22rem;
		line-height: 0.22rem;
		margin-top: 13px;
		font-size: 0.16rem;
	}
	.right .pinlun{
		margin-top: 7px;
		color: #616161;
	}
	.right .price{
		margin-top: 11px;
	}
	.right .price span{
		color: #ff8300;
		font-size: 0.2rem;
	}
	.right .price .adress{
		font-size: 0.12rem;
		color: #616161;
		float: right;
	}
	.right .tishi{
		margin-top: 24px;
		margin-right: 12px;
		padding: 2px 5px;
		color: #f55;
		background: #fff9f9;
	}
	.search{
		display: block;
		padding: 10px 0;
		color: #00afc7;
		font-size: .14rem;
		line-height: .2rem;
	}
</style>