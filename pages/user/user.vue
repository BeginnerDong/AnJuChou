<template>
	<view>
		<view style="height:var(--status-bar-height)"></view>
		<view class="head p-s top-0 text-c">
			个人
			<view class="p-aXY d-flex j-end p-3">
				<image src="../../static/images/my-icon1.png" class="wh34"
				@click="Router.navigateTo({route:{path:'/pages/apply/apply'}})"></image>
				<image src="../../static/images/my-icon2.png" class="wh32 ml-5"
				@click="Router.navigateTo({route:{path:'/pages/news/news'}})"></image>
			</view>
		</view>
		
		<view class="flex line-h px-2 py-3">
			<image src="../../static/images/my-icon.png"  class="wh126 radius-5"></image>
			<view class="pl-2">
				<view class="font-34 font-w pb-3">登录/注册</view>
				<view class="font-22 color9"
				@click="Router.navigateTo({route:{path:'/pages/login/login'}})">点击登录</view>
			</view>
		</view>
		
		<view class="px-2 p-r">
			<image src="../../static/images/my-img.png" mode="widthFix"></image>
			<view class="p-aXY color flex2 line-h">
				<view class="flex4 w-33 p-r bb"
				@click="Router.navigateTo({route:{path:'/pages/user-assets/user-assets'}})">
					<view class="font-36 font-w">5,252.32</view>
					<view class="font-22 pt-2">资产 ></view>
				</view>
				<view class="flex4 w-33 p-r bb"
				@click="Router.navigateTo({route:{path:'/pages/user-assets/user-assets'}})">
					<view class="font-36 font-w">5,252.32</view>
					<view class="font-22 pt-2">收益 ></view>
				</view>
				<view class="w-33">
					<view class="btn60-c"
					@click="Router.navigateTo({route:{path:'/pages/recharge/recharge'}})">充值</view>
				</view>
			</view>
		</view>
		
		<view class="flex2 line-h pt-5 mt-1 font-26 px-1">
			<view class="item flex4"
			@click="Router.navigateTo({route:{path:'/pages/user-setting/user-setting'}})">
				<image src="../../static/images/my-icon6.png" class="icon1"></image>
				<view class="pt-3">账户设置</view>
			</view>
			<view class="item flex4"
			@click="Router.navigateTo({route:{path:'/pages/user-project/user-project'}})">
				<image src="../../static/images/my-icon4.png" class="icon2"></image>
				<view class="pt-3">投资项目</view>
			</view>
			<view class="item flex4"
			@click="Router.navigateTo({route:{path:'/pages/user-deal/user-deal'}})">
				<image src="../../static/images/my-icon3.png" class="icon3"></image>
				<view class="pt-3">交易记录</view>
			</view>
			<view class="item flex4"
			@click="Router.navigateTo({route:{path:'/pages/user-recommend/user-recommend'}})">
				<image src="../../static/images/my-icon5.png" class="icon4"></image>
				<view class="pt-3">邀请好友</view>
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
			<view class="item" @click="Router.redirectTo({route:{path:'/pages/change/change'}})">
				<image src="../../static/images/nabar3.png" mode=""></image>
				<view>转让区</view>
			</view>
			<view class="item on">
				<image src="../../static/images/nabar4-a.png" mode=""></image>
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
.head{line-height: 80rpx;}
	
.color{color: #4e3616;}
.w-33{width: 33.33%;}
.btn60-c{background-color: #4e3616;width: 120rpx;}
.bb::before{content: '';border-left: 1px solid #d6cfb0;height: 40rpx;position: absolute;right: 0;top: 50%;margin-top: -20rpx;}

.icon1{width:69rpx;height: 56rpx;}
.icon2{width:60rpx;height: 54rpx;}
.icon3{width:51rpx;height: 60rpx;}
.icon4{width:58rpx;height: 58rpx;}
</style>
