<template>
	<div class="about">
		<div class="left">
			<span>About</span>
			<p>我们的理念</p>
			<p>最领先的响应式自助建站平台，我们的流线式网页布局设计方案和可视化图文内容编辑模式让网站制作和维护成为一件轻松惬意的事。无论您是普通互联网用户， 还是专业网站制作人员，都能使用起飞页设计出最具专业水准的网站</p>
			<button @mouseover="move($event)" @mouseout="over($event)">MORE</button>
		</div>
		<div class="right">
			<ul>
				<li v-for="i in arr">
					<img :src=i>
				</li>
			</ul>
		</div>
	</div>
</template>

<script>
	export default{
		data(){
			return{
				arr:[
					'https://ccdn.goodq.top/caches/90800e7c26d8ce3a5a2ca07c1f6743b9/aHR0cDovLzU4ODA1MGMwYTI4MDEudDc0LnFpZmVpeWUuY29tL3FmeS1jb250ZW50L3VwbG9hZHMvMjAxNy8wMy80YmRjMzdmZmJiY2ZmNjU5MjgyNjE4YTllZjYyOTcwZC01MDB4NDUwLmpwZw_p_p100_p_3D_p_p100_p_3D.jpg',
					'https://ccdn.goodq.top/caches/90800e7c26d8ce3a5a2ca07c1f6743b9/aHR0cDovLzU4ODA1MGMwYTI4MDEudDc0LnFpZmVpeWUuY29tL3FmeS1jb250ZW50L3VwbG9hZHMvMjAxNy8wMy9mOTgzNTNmMzMwOGNjZjJjMDlkYzg2MjIxNzgyMjllYS01MDB4NDUwLmpwZw_p_p100_p_3D_p_p100_p_3D.jpg',
					'https://ccdn.goodq.top/caches/90800e7c26d8ce3a5a2ca07c1f6743b9/aHR0cDovLzU4ODA1MGMwYTI4MDEudDc0LnFpZmVpeWUuY29tL3FmeS1jb250ZW50L3VwbG9hZHMvMjAxNy8wNy8xNTAwODkwODUzNTk3NWM2ZTVkYjY0Nzk0NzgtNTAweDQ1MC5wbmc_p_p100_p_3D.png',
					'https://ccdn.goodq.top/caches/90800e7c26d8ce3a5a2ca07c1f6743b9/aHR0cDovLzU4ODA1MGMwYTI4MDEudDc0LnFpZmVpeWUuY29tL3FmeS1jb250ZW50L3VwbG9hZHMvMjAxNy8wNy82NzVlYTIyMmVmZWY1OGIwYmU4YWRhMDkxODBjMmEyZC01MDB4NDUwLmpwZw_p_p100_p_3D_p_p100_p_3D.jpg',
					'https://ccdn.goodq.top/caches/90800e7c26d8ce3a5a2ca07c1f6743b9/aHR0cDovLzU4ODA1MGMwYTI4MDEudDc0LnFpZmVpeWUuY29tL3FmeS1jb250ZW50L3VwbG9hZHMvMjAxNy8wNy8xOTZiOWJkYTFmNThmNDY5Yjc4MGI4NzUzNWUzYWE5My01MDB4NDUwLmpwZw_p_p100_p_3D_p_p100_p_3D.jpg',
					'https://ccdn.goodq.top/caches/90800e7c26d8ce3a5a2ca07c1f6743b9/aHR0cDovLzU4ODA1MGMwYTI4MDEudDc0LnFpZmVpeWUuY29tL3FmeS1jb250ZW50L3VwbG9hZHMvMjAxNy8xMC9kMmIzZmViMTcxZDgwOTQyZTY3MzQxMjIxZjM4OWQ4ZC01MDB4NDUwLmpwZw_p_p100_p_3D_p_p100_p_3D.jpg'
				]
			}
		},
		methods:{
			move(e){
				e.target.style.backgroundColor='rgb(239, 193, 124)',
				e.target.style.color='black'
			},
			over(e){
				e.target.style.backgroundColor='',
				e.target.style.color=''
			}
		}
	}
</script>

<style scoped>
	.about{
		width: 100%;
		height: 505px;
		background: black;
	}
	.left{
		width: 25%;
		height: auto;
		float: left;
		padding-left: 8%;
	}
	.right{
		width: 67%;
		height: 100%;
		float: left;
	}
	.left p:nth-child(2){
		color: #efc17c;
		font-size: 20px;
		margin-top: -10px;
		margin-bottom: 40px;
	}
	.left p:nth-child(3){
		width: 228px;
		height: auto;
		font-size: 14px;
		line-height: 24px;
	}
	.left span{
		display: block;
		color: white;
		font-size: 60px;
		margin-top: 50px;
	}
	.left button{
		background: black;
		border: 1px solid rgb(239, 193, 124);
		color: rgb(239, 193, 124);
		padding: 5px 60px;
		font-size: 14px;
		font-family: "times new roman";
		margin-top: 40px;
	}
	.right ul{
		width: 100%;
		height: 100%;
	}
	.right ul li{
		width: 33.33%;
		height: 50%;
		float: left;
	}
	.right ul li img{
		width: 100%;
		height: 100%;
		cursor: pointer;
	}
</style>