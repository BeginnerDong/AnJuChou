<template>
	<view>
		
		<view class="mt-2 px-3 pt-4 pb-3 bg-white line-h radius10 mx-2"
		@click="Router.navigateTo({route:{path:'/pages/detail/detail'}})">
			<view class="pb-3 flex1">
				<view class="d-flex a-end flex-1">
					<view class="font-32 font-w">招商泽瑞</view>
					<view class="pl-3">净值 <text class="colorR font-32 font-w">1.205</text></view>
				</view>
				<view class="btn60 Mgb"
				@click="Router.navigateTo({route:{path:'/pages/buy/buy'}})">买入</view>
				<!-- <view class="color9">已完成</view> -->
			</view>
			<view class="flex2 py-3 radius10 box">
				<view class="flex4">
					<view class="font-24 color6 pb-2">份额</view>
					<view class="font-32 colorM1 font-w">10000</view>
				</view>
				<view class="flex4">
					<view class="font-24 color6 pb-2">当前价</view>
					<view class="font-32 colorM1 font-w">12050</view>
				</view>
				<view class="flex4">
					<view class="font-24 color6 pb-2">转让价(-0.5%)</view>
					<view class="font-32 colorM1 font-w">10000</view>
				</view>
			</view>
		</view>
		
		
		<view style="height: 130rpx;"></view>
		<!-- footer -->
		<view class="footer">
			<view class="item" @click="Router.redirectTo({route:{path:'/pages/index/index'}})">
				<image src="../../static/images/nabar1.png" mode=""></image>
				<view>首页</view>
			</view>
			<view class="item" @click="Router.redirectTo({route:{path:'/pages/project/project'}})">
				<image src="../../static/images/nabar2.png" mode=""></image>
				<view>项目</view>
			</view>
			<view class="item on">
				<image src="../../static/images/nabar3-a.png" mode=""></image>
				<view>转让区</view>
			</view>
			<view class="item" @click="Router.redirectTo({route:{path:'/pages/user/user'}})">
				<image src="../../static/images/nabar4.png" mode=""></image>
				<view>个人</view>
			</view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				Router:this.$Router
			}
		},
		methods: {
			
		}
	}
</script>
<style>
page{background-color: #f5f5f5;}
</style>
<style scoped>
.box{background-color: #f4f6fa;}
.btn60{width: 110rpx;}
</style>
