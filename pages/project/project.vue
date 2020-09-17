<template>
	<view>
		
		<view class="px-2 py-2 flex line-h">
			<view>西安</view>
			<image src="../../static/images/project-icon.png" class="xl-icon ml-1"></image>
		</view>
		
		<view class="mx-2 radius10 overflow-h shadow p-r mb-5"
		@click="Router.navigateTo({route:{path:'/pages/detail/detail'}})">
			<view class="sign">进行中</view>
			<image src="../../static/images/home-img1.png" class="img1"></image>
			<view class="py-3 px-2 line-h">
				<view class="font-30 color1 font-w pb-2">准备金筹款</view>
				<view class="flex1 font-24 color4 pb-3">
					<view>当前筹款进度：</view>
					<view class="speed"></view>
					<view>15%</view>
				</view>
				<view class="price font-32">562万</view>
			</view>
		</view>
		<view class="mx-2 radius10 overflow-h p-r mb-5 flex1" v-for="v in 2" :key="v"
		@click="Router.navigateTo({route:{path:'/pages/detail/detail'}})">
			<view class="sign">进行中</view>
			<!-- <view class="sign bg90">已完成</view> -->
			<image src="../../static/images/home-img2.png" class="img2"></image>
			<view class="pl-2 line-h flex-1 h200 flex5 py-1">
				<view class="font-30 color1 font-w pb-2">准备金筹款</view>
				<view class="font-24 color4 pb-3">
					<view class="pb-2">当前筹款进度：15%</view>
					<view class="speed"></view>
				</view>
				<view class="price font-32">562万</view>
			</view>
		</view>
		
		
		
		<view style="height: 130rpx;"></view>
		<!-- footer -->
		<view class="footer">
			<view class="item" @click="Router.redirectTo({route:{path:'/pages/index/index'}})">
				<image src="../../static/images/nabar1.png" mode=""></image>
				<view>首页</view>
			</view>
			<view class="item on">
				<image src="../../static/images/nabar2-a.png" mode=""></image>
				<view>项目</view>
			</view>
			<view class="item" @click="Router.redirectTo({route:{path:'/pages/change/change'}})">
				<image src="../../static/images/nabar3.png" mode=""></image>
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

<style>page{background-color: #fff;}</style>
<style scoped>
.img1{height: 320rpx;width: 100%;}
.img2{height: 200rpx;width: 260rpx;}
.h200{height: 200rpx;}
.bg90{background-color: #909090;}

.speed{width: 400rpx;}
.speed::before{width: 15%;}
</style>
