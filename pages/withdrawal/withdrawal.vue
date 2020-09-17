<template>
	<view class="px-2">
		
		<view class="p-3 mt-3 bg-white radius10 line-h flex1">
			<view>
				<view class="font-30 pb-3 font-w">中国银行</view>
				<view class="color6 font-26">6325124****253589</view>
			</view>
			<image src="../../static/images/thelogin-icon2.png" class="R-icon"></image>
		</view>
		
		<view class="px-2 bg-white mt-3 line-h radius10 pt-3">
			<view class="py-6 color6 mb-4">提现金额</view>
			<view class="flex py-4 bB-e1">
				<view class="font-50 font-w">￥</view>
				<input type="number" value="" placeholder="" />
			</view>
			<view class="font-24 color9 py-3">可用余额0.00元</view>
		</view>
		
		<view class="btn80 Mgb">确定</view>
		
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
<style>page{background-color: #f5f5f5;}</style>
<style scoped>
.btn80{margin-top: 100rpx;}
.R-icon{width: 15rpx;height: 30rpx;}
</style>
