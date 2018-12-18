<template>
	<swiper :options="swiperOption">
	    <!-- slides -->
	    <swiper-slide v-for="item of imgList" :key="item.src">
	    	<img :src="item.src">
	    </swiper-slide>
	    <!-- Optional controls -->
	    <div class="swiper-pagination" slot="pagination"></div>
	 </swiper>
</template>
<script>
  export default {
    data() {
      return {
        swiperOption: {
        	pagination: {
				el:".swiper-pagination"
			},
			loop:true
        },
        imgList:[
        	{
        		id:0,
        		src:require("@/assets/images/1.jpg")
        	},
        	{
        		id:1,
        		src:require("@/assets/images/2.jpg")
        	},
        	{
        		id:2,
        		src:require("@/assets/images/3.jpg")
        	},
        	{
        		id:3,
        		src:require("@/assets/images/4.jpg")
        	},
        	{
        		id:4,
        		src:require("@/assets/images/5.jpg")
        	},
        	{
        		id:5,
        		src:require("@/assets/images/6.jpg")
        	},
        	{
        		id:6,
        		src:require("@/assets/images/7.jpg")
        	},
        	{
        		id:7,
        		src:require("@/assets/images/8.jpg")
        	},
        	{
        		id:8,
        		src:require("@/assets/images/9.jpg")
        	},
        	{
        		id:9,
        		src:require("@/assets/images/10.jpg")
        	}
        ]
      }
    }
  }
</script>
<style scoped>
	img{
		width: 100%;
	}
</style>