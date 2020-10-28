<template>
	<div class="tabbar">
		<slot></slot>
	</div>
</template>

<script>
	export default{
		name:"tabbar"
	}
</script>

<style >
	.tabbar{
		height: 50px;
		display: flex;
		justify-content: space-around;
		font-size: 13px;
	}
</style>
