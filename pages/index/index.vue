<template>
	<view>
		
		<view>
			<image src="../../static/images/home-img.png" class="img"></image>
		</view>
		<view class="px-2 pt-4">
			<view class="font-36 color1 pb-3 line-h font-w">安居筹介绍</view>
			<view class="color4 line-h-md bB-f5 py-4">安居筹介绍安居筹介绍安居筹介绍安居筹介绍安居筹介绍安居筹介绍安居筹介绍安居筹介绍安居筹介绍</view>
			<view class="font-30 line-h py-4 flex1"
			@click="Router.navigateTo({route:{path:'/pages/contactUs/contactUs'}})">
				<view>联系我们</view>
				<image src="../../static/images/thelogin-icon2.png" class="R-icon"></image>
			</view>
		</view>
		<view class="f5Bj-H20"></view>
		
		<view class="list mb-2">
			<view class="li" :class="liCurr==0?'on':''" @click="changeLi(0)">进行项目</view>
			<view class="li" :class="liCurr==1?'on':''" @click="changeLi(1)">完结项目</view>
		</view>
		
		<view class="mx-2 radius10 overflow-h shadowM p-r mb-5"
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
			<view class="item on">
				<image src="../../static/images/nabar1-a.png" mode=""></image>
				<view>首页</view>
			</view>
			<view class="item" @click="Router.redirectTo({route:{path:'/pages/project/project'}})">
				<image src="../../static/images/nabar2.png" mode=""></image>
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
				Router:this.$Router,
				is_show: false,
				liCurr:0
			}
		},
		onLoad() {
			const self = this;
			// self.$Utils.loadAll(['getMainData'], self);
		},
		methods: {
			
			changeLi(i){
				const self = this;
				self.liCurr = i;
			},
			
			getMainData() {
				const self = this;
				console.log('852369')
				const postData = {};
				postData.tokenFuncName = 'getProjectToken';
				self.$apis.orderGet(postData, callback);
			}
		}
	};
</script>
<style>page{background-color: #fff;}</style>
<style scoped>
.img{width: 100%;height: 400rpx;}
.li{width: 23%;font-size: 30rpx;color: #222;padding: 40rpx 0;}
.list{margin: 0;}
.list .on{font-size: 32rpx;font-weight: 800;}
.list .on::before{width: 40rpx;height: 6rpx;border-radius: 3rpx;bottom: 30rpx;left: 50%;margin-left: -20rpx;}

.img1{height: 320rpx;width: 100%;}
.img2{height: 200rpx;width: 260rpx;}
.h200{height: 200rpx;}
.bg90{background-color: #909090;}

.speed{width: 400rpx;}
.speed::before{width: 15%;}
</style>