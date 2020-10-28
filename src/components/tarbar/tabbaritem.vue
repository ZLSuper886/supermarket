<template>
	<div class="tabbaritem" @click="itemclick">
	    <div v-if="!isActive"><slot name="img" ></slot></div>	
		<div v-else><slot  name="img2"></slot></div>
		<div :style="activeStyle"><slot name="text" ></slot></div>
	</div>	
</template>

<script>
	export default{
		name:"tabbaritem",
		props:{
			path:String,
			activeColor:{
				type:String,
				default:"red"
			}
		},
		data(){
			return{
				// isActive:true,
			}
		},
		computed:{
			isActive(){
				return this.$route.path.indexOf((this.path))!==-1
			},
			activeStyle(){
				return this.isActive?{color:this.activeColor}:{}
			}
		},
		methods:{
			itemclick(){
				this.$router.replace(this.path)
			}
		}
	}
</script>

<style scoped>
	.tabbaritem img{
		margin-top: 3px;
		vertical-align: middle;
	}
	/* .active{
		color: #42B983;
	} */
</style>
