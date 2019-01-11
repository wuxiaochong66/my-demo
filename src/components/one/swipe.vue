<template>
	    <div class="swiper-container">
		    <div class="swiper-wrapper">
		        <div class="swiper-slide" v-for="i in arr"><img :src=i></div>
		    </div>
		    <!-- 如果需要分页器 -->
		    <div class="swiper-pagination"></div>
		    
		    <!-- 如果需要导航按钮 -->
		    <div class="swiper-button-prev"></div>
		    <div class="swiper-button-next"></div>
		    
		    <!-- 如果需要滚动条 -->
		    <div class="swiper-scrollbar"></div>
		</div>
</template>

<script>
	import Swiper from 'swiper';
	export default {	
	    data () {
		    return {
		    	arr:["https://ccdn.goodq.top/caches/90800e7c26d8ce3a5a2ca07c1f6743b9/aHR0cDovLzU4ODA1MGMwYTI4MDEudDc0LnFpZmVpeWUuY29tL3FmeS1jb250ZW50L3VwbG9hZHMvMjAxNy8xMC8zMjQwODI4NmFmYTZjZGI2MzQ1MzA4M2NmN2M4MmViOC5qcGc_p_p100_p_3D.jpg","https://ccdn.goodq.top/caches/90800e7c26d8ce3a5a2ca07c1f6743b9/aHR0cDovLzU4ODA1MGMwYTI4MDEudDc0LnFpZmVpeWUuY29tL3FmeS1jb250ZW50L3VwbG9hZHMvMjAxNy8xMC9iYjg4MDlmMzYyOGNhYmI3ZGY2YjRjYThlZTM2MTgyNS5qcGc_p_p100_p_3D.jpg"]
		    }
		},
		mounted(){
		    new Swiper ('.swiper-container', {
			    loop: true,
			    autoplay:{
			    	delay: 3000,
				    disableOnInteraction: false,
			    },
			    // 如果需要前进后退按钮
			    nextButton: '.swiper-button-next',
			    prevButton: '.swiper-button-prev'
			})        
		},
		methods:{
			
		}
	}
</script>

<style scoped>
	.swiper-container {
        width: 100%;
        height: 592px;
    }
    .swiper-slide img{
    	width: 100%;
    	height: 100%;
    }
</style>