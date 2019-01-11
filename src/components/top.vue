<template>
	<div id="top">
		<div class="left">
			<img src="https://ccdn.goodq.top/caches/90800e7c26d8ce3a5a2ca07c1f6743b9/aHR0cDovLzU4ODA1MGMwYTI4MDEudDc0LnFpZmVpeWUuY29tL3FmeS1jb250ZW50L3VwbG9hZHMvMjAxNy8xMC83YWVmMWU1MzA3ZGIyNTJlNDAyMjBhNzM3MjEzZWE1OC5wbmc_p_p100_p_3D.png">
		</div>
		<div class="right">
			<ul>
				<li v-for="(i,index) in arr" @click="dianji(index)">{{i}}</li>
			</ul>
		</div>
		<component :is="con"></component>
	</div>
</template>

<script>
	import one from "./one";
	import two from "./two";
	import three from "./three";
	
	export default{
		data(){
			return{
				con:"one",
				arr:["首页","商品分类","商城资讯","品牌介绍","联系我们"],
				arr1:['one','two','three'],
				activeClass: 0,
				active: 'active'
			}
		},
		components:{
			one,
			two,
			three
		},
		methods:{
			dianji(index){
				this.con=this.arr1[index],
				this.activeClass = index;
			}
		}
	}
</script>

<style scoped="scoped">
	#top{
		width: 100%;
		height: 95px;
		display: block;
		background: black;
	}
	.left{
		width: 30%;
		height: 95px;
		float: left;
	}
	.left img{
		width: 124px;
		height: 55px;
		margin-top: 20px;
		margin-left: 35px;
		cursor: pointer;
	}
	.right{
		width: 70%;
		height: 95px;
		float: left;
	}
	.right ul{
		width: 70%;
		height: 95px;
		float: right;
	}
	.right ul li{
		width: 20%;
		height: 95px;
		line-height: 95px;
		float: left;
		list-style: none;
		cursor: pointer;
		color: #efc17c;
		font-size: 14px;
	}
	/*.active {*/
		/*background: red;*/
		/*color: red;*/
	/*}*/
</style>