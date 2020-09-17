<template>
	<view class="box">
		
		<view class="font-44 font-w top">找回密码</view>
		
		<input type="text" value="" placeholder="账号" />
		<view class="flex1 colorM yzm">
			<input type="text" value="" placeholder="验证码" />
			<view class="pt-3 font-w">获取验证码</view>
		</view>
		<input type="text" value="" placeholder="密码" />
		
		<view class="flex1 pt-3">
			<!-- <image src="../../static/images/registered-icon.png" class="wh34"></image> -->
			<image src="../../static/images/registered-icon1.png" class="wh34"></image>
			<view class="font-24 pl-2 flex-1">
				我已阅读并同意
				<text class="colorM">《安居筹用户协议》，</text>
				<text class="colorM">《安居筹隐私政策》</text>
			</view>
		</view>
		
		<view class="btn80 Mgb">确定</view>
		
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
.btn80{margin-top: 100rpx;}
.yzm{border-bottom: 1px solid #f5f5f5;}
.yzm input{border: none;}
</style>
