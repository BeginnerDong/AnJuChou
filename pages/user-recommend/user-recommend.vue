<template>
	<view>
		
		<view class="mx-2 mt-3 p-3 radius10 top">
			<view class="bg-white radius10 py-4 flex">
				<view class="flex4 w-50 p-r one">
					<view class="font-36 font-w">26</view>
					<view class="font-22 color9">好友注册</view>
				</view>
				<view class="flex4 w-50">
					<view class="font-36 font-w">265253.36</view>
					<view class="font-22 color9">累计额度</view>
				</view>
			</view>
		</view>
		
		<view class="bg-f5 radius10 overflow-h mx-a pb-5 box">
			<view class="Mgb1 p-3 colorf flex">
				<image src="../../static/images/recommended-icon.png" class="wh33 mr-1"></image>
				<view>推荐好友注册</view>
			</view>
			<image src="../../static/images/recommended-img.png" class="ewm"></image>
			<view class="btn70 Mgb">保存图片</view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>
<style>page{background-color: #fff;}</style>
<style scoped>
.top{background-image: linear-gradient(to right,#5270CD ,#3650A3);box-shadow: 0 5rpx 16rpx rgba(82, 112, 250, 0.5);}
.one::before{content: '';border-right: 1px solid #f5f5f5;height: 40rpx;position: absolute;right: 0;top: 50%;margin-top: -20rpx;}
.box{width: 600rpx;margin-top: 60rpx;}
.ewm{width: 340rpx;height: 340rpx;margin: 100rpx auto 60rpx;}
.btn70{width: 300rpx;border-radius: 0;}
</style>
