<template>
	<div id="index">
		<topt></topt>
		<top></top>
	</div>
</template>

<script>
	import top from "../components/top"
	import topt from "../components/topt"
	export default{
		data(){
			return{
				
			}
		},
		methods:{
			
		},
		components:{
			topt,
			top
		}
	}
</script>

<style>
	*{
		margin: 0;
		padding: 0;
	}
	#index{
		width: 100%;
		height: auto;
	}
</style>