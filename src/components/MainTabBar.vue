<template>
	<tarbar>
		<tabbaritem  path="/home" activeColor="greenYellow">
			<img slot="img" src="../assets/img/shouye0.png" width="25" alt="">
			<img slot="img2" src="../assets/img/shouye1.png" width="25" alt="">
			<div slot="text">首页</div>
		</tabbaritem>
		<tabbaritem path="/category" activeColor="greenYellow">
			<img slot="img" src="../assets/img/shouye0.png" width="25" alt="">
			<img slot="img2" src="../assets/img/shouye1.png" width="25" alt="">
			<div slot="text">分类</div>
		</tabbaritem>
		<tabbaritem path="/profile" activeColor="greenYellow">
			<img slot="img" src="../assets/img/shouye0.png" width="25" alt="">
			<img slot="img2" src="../assets/img/shouye1.png" width="25" alt="">
			<div slot="text">我的</div>
		</tabbaritem>
		<tabbaritem path="/cart" activeColor="greenYellow">
			<img slot="img" src="../assets/img/shouye0.png" width="25" alt="">
			<img slot="img2" src="../assets/img/shouye1.png" width="25" alt="">
			<div slot="text">购物</div>
		</tabbaritem>
	</tarbar>
</template>

<script>
	import tarbar from "./tarbar/tabbar.vue"
	import tabbaritem from "./tarbar/tabbaritem.vue"
	export default{
		name:"App",
		components: {
			tarbar,
			tabbaritem
		}
	}
</script>

<style>
</style>
