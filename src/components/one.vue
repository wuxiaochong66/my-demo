<template>
	<div id="one">
		<swipe></swipe>
		<about></about>
		<the></the>
	</div>
</template>

<script>
	import swipe from "./one/swipe"
	import about from "./one/about"
	import the from "./one/the"
	export default{
		data(){
			return{
				
			}
		},
		methods:{
			
		},
		components:{
			swipe,
			about,
			the
		}
	}
</script>

<style scoped>
	#one{
		width: 100%;
		height: auto;
		float: left;
	}
</style>