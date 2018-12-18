<template>
	<div class="w3">
		<h3>周末去哪儿</h3>
		<ul>
			<li v-for="item of liList">
				<img :src="item.src" alt="">
				<div class="wenzi">					
					<div>{{item.title}}</div>
					<p>{{item.content}}</p>
				</div>
			</li>
		</ul>
	</div>
</template>
<script>
	export default {
		data(){
			return{
				liList:[
					{
						id:0,
						src:"http://img1.qunarzz.com/sight/source/1505/74/98a840f2a881b.jpg_r_640x214_1bf94c8e.jpg",
						title:"西安温泉季",
						content:"养生、养性、养心的理想之地，曲径通幽，鸟语花香，让您在远离喧嚣之地享受终南隐士生活。"
					},
					{
						id:1,
						src:"http://img1.qunarzz.com/sight/source/1606/fa/1fca5cab2918f0.jpg_r_640x214_6902e556.jpg",
						title:"咸阳必游TOP10",
						content:"养生、养性、养心的理想之地，曲径通幽，鸟语花香，让您在远离喧嚣之地享受终南隐士生活。"
					},
					{
						id:2,
						src:"http://img1.qunarzz.com/sight/source/1506/26/5e8fad4a4a4be2.jpg_r_640x214_8d055589.jpg",
						title:"山外有山",
						content:"这里曾是太乙真人修炼地，唐王李世民的避暑消夏胜地，山清水秀、景色如画、气候凉爽"
					},
					{
						id:3,
						src:"http://img1.qunarzz.com/sight/source/1511/14/1cf5dc2ecbfc16.jpg_r_640x214_b4b3a58a.jpg",
						title:"醉美丝路行",
						content:"情系西北，中国梦丝路行"
					},
					{
						id:4,
						src:"http://img1.qunarzz.com/sight/source/1509/1c/6067358591f975.jpg_r_640x214_df0e5390.jpg",
						title:"那些不能忘却的古镇",
						content:"陕西的丽江，这里有丰富的历史文化资源，古老石砌的巷道，诉说着往日的兴盛与辉煌"
					}
				]
			}
		}
	}
</script>
<style scoped>
	.w3{
		text-align: left;
	}
	h3{
		height: 0.4rem;
		padding-left: 0.13rem;
		line-height: 0.4rem;
		color: #212121;
		font-size: 0.14rem;
		font-weight: normal;
	}
	ul{
		background: #fff;
	}
	img{
		width: 100%;
	}
	.wenzi{
		padding: 7px 10px 10px 10px;
	}
	.wenzi div,.wenzi p{
		overflow: hidden;
		color: #212121;
		font-size: .14rem;
		line-height: .24rem;
		white-space: nowrap;
		text-overflow: ellipsis;
	}
	.wenzi p{
		color: #616161;
		font-size: 12px;
		padding-right: 0.7rem;
	}
</style>