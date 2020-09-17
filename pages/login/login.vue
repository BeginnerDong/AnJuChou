<template>
	<view class="box">
		
		<view class="font-44 font-w top">登录账号</view>
		
		<input type="text" value="" placeholder="账号" placeholder-style="font-size:26rpx;"/>
		<input type="text" value="" placeholder="密码" />
		
		<view class="btn80 Mgb">确定</view>
		<view class="flex2 py-3 font-26 color6">
			<view @click="Router.navigateTo({route:{path:'/pages/register/register'}})">没有账号？去注册 ></view>
			<view @click="Router.navigateTo({route:{path:'/pages/password/password'}})">找回密码 ></view>
		</view>
		
		<view class="p-fX bottom-0">
			<view class="flex1 font-26 color6 pb-5">
				<view class="line"></view>
				<view>第三方登录</view>
				<view class="line"></view>
			</view>
			<view class="flex0 pb-5">
				<!-- <image src="../../static/images/thelogin-icon.png" class="QQ"></image> -->
				<image src="../../static/images/thelogin-icon3.png" class="QQ"></image>
				<image src="../../static/images/thelogin-icon1.png" class="wx"></image>
				<!-- <image src="../../static/images/thelogin-icon4.png" class="wx"></image> -->
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
		onLoad() {
			
		},
		methods: {
			
		}
	}
</script>
<style>page{background-color: #fff;}</style>
<style scoped>
.box{width: 600rpx;margin: 0 auto;}
.top{padding: 140rpx 0 40rpx;}
input{width: 100%;padding: 0;padding: 60rpx 0 30rpx;border-bottom: 1px solid #f5f5f5;font-size: 26rpx;}
input::-webkit-input-placeholder{font-size: 26rpx;}
.btn80{margin-top: 100rpx;}

.line{width: 35%;border-top: 1px solid #f5f5f5;}
.QQ{width: 50rpx;height: 59rpx;margin: 0 75rpx;}
.wx{width: 66rpx;height: 55rpx;margin: 0 75rpx;}
</style>