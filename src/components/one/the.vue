<template>
	<div class="the">
		<div class="left">
			<img src="https://ccdn.goodq.top/caches/90800e7c26d8ce3a5a2ca07c1f6743b9/aHR0cDovLzU4ODA1MGMwYTI4MDEudDc0LnFpZmVpeWUuY29tL3FmeS1jb250ZW50L3VwbG9hZHMvMjAxNy8wMy80YmRjMzdmZmJiY2ZmNjU5MjgyNjE4YTllZjYyOTcwZC5qcGc_p_p100_p_3D.jpg">
		</div>
		<div class="right">
			<p>THE CHOICE OF THE LUXURIOUS</p>
			<p>全新Dior迪奥小姐香氛，散发感性迷人的高订气质：<br>
格拉斯五月玫瑰与土耳其大马士革玫瑰打造精致蕾丝裙装，卡拉布里亚佛手柑的柑橘香调如清新“蝴蝶结”。法属圭亚那蔷薇木和留尼汪岛粉红胡椒交织共舞，为这件高订“刺绣”更添生动辛辣。繁花谱写的爱情宣言，带给你一见钟情的芬芳气息。</p>
			<button @mouseover="move($event)" @mouseout="over($event)">MORE</button>
		</div>
	</div>
</template>

<script>
	export default{
		data(){
			return{
				
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
	.the{
		width: 100%;
		height: 737px;
		background: #1e1e1e;
	}
	.left{
		width: 46%;
		height: 100%;
		float: left;
	}
	.left img{
		width: 500px;
		height: 500px;
		margin-top: 130px;
		float: right;
	}
	.right{
		width: 54%;
		height: 100%;
		float: left;
	}
	.right p:nth-child(1){
		color: rgb(255, 255, 255);
		font-size: 22px;
		font-family: times new roman;
	}
	.right p:nth-child(2){
		letter-spacing: 2px;
		color:#A9A9A9;
		font-size: 12px;
	}
	.right button{
		background: black;
		border: 1px solid rgb(239, 193, 124);
		color: rgb(239, 193, 124);
		padding: 5px 60px;
		font-size: 14px;
		font-family: "times new roman";
		margin-top: 40px;
	}
</style>