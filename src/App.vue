<template>
	<div id="app">
		<Layout>
			<Header :style="{background:'#fff', padding:'0', height:'60px'}">
				<navbar />
			</Header>
			<div class="x-placeholder"></div>
			<Layout>
				<Sider :style="{background:'#fff', borderRight:'1px solid #dddddd'}">
					<Tree :data="data1" class="tree-left"></Tree>
				</Sider>
				<Content :style="{background:'#fff'}">
					<div class="side-line"></div>
				</Content>
			</Layout>
			<div class="x-placeholder"></div>
			<Footer :style="{background:'#fff', borderTop:'1px solid #dddddd', display:'flex'}">
				<div class="">
					<p>
						Leep's Blog. ©2019
						<!-- <br> -->
						Powered By 
						<a href="https://www.iviewui.com/">iView</a>
						<br>
						<br>
						友情链接:
						<a href="https://www.shi-ci.com/">中华诗词</a>
					</p>
				</div>
				<div class="y-placeholder"></div>
				<Button shape="circle" size="large"  :style="{height:'35px', width:'35px'}" icon="logo-github" to="https://github.com/pqs921209/" ></Button>
			</Footer>
		</Layout>

	</div>
</template>

<script>
import navbar from "./components/navbar/navbar";
// import sidebar from "./components/sidebar/sidebar";

export default {
	name: "app",
	components: {
		navbar,
		// sidebar
	},
	data() {
		return {
			// 左侧菜单数据
			data1: [
				{
					title: 'parent 1',
					expand:true,
					children: [
						{
							title: 'parent 1-1',
							children: [
								{
									title: 'leaf 1-1-1'
								},
								{
									title: 'leaf 1-1-2'
								}
							]
						},
						{
							title: 'parent 1-2',
							children: [
								{
									title: 'leaf 1-2-1'
								},
								{
									title: 'leaf 1-2-1'
								}
							]
						}
					]
				},
				{
					title: 'parent 2',
					children:[
						{
							title: 'leaf 2-1'
						}
					]
				}
			]
		}
	},
};
</script>

<style>
#app {
	font-family: "Helvetica Neue", Helvetica, "PingFang SC", "Hiragino Sans GB","Microsoft YaHei", "微软雅黑", Arial, sans-serif;
}
.ivu-layout-header{
	background: #fff;
	padding: 0;
}
.x-placeholder{
	background: #fff;
	height: 25px;
}
.y-placeholder{
	background: #fff;
	width: 10%;
}
.tree-left{
	margin-left: 20px;
}
</style>
