<template>
	<view>
		
		<view class="px-2 bg-white mt-2 line-h">
			<view class="font-30 py-6">充值金额</view>
			<view class="flex py-4">
				<view class="font-50 font-w">￥</view>
				<input type="number" value="" placeholder="" />
			</view>
		</view>
		
		<view class="mt-2 bg-white px-2">
			<view class="font-34 py-4 font-w">付款方式</view>
			<view class="flex1 pb-4">
				<image src="../../static/images/pay-icon3.png" class="wh34"></image>
				<view class="flex-1 px-2">微信支付</view>
				<image src="../../static/images/pay-icon1.png" class="wh34"></image>
				<!-- <image src="../../static/images/pay-icon2.png" class="wh34"></image> -->
			</view>
			<view class="flex1 pb-4">
				<image src="../../static/images/pay-icon5.png" class="wh34"></image>
				<view class="flex-1 px-2">支付宝支付</view>
				<!-- <image src="../../static/images/pay-icon1.png" class="wh34"></image> -->
				<image src="../../static/images/pay-icon2.png" class="wh34"></image>
			</view>
			<view class="flex1 pb-4">
				<image src="../../static/images/pay-icon4.png" class="wh34"></image>
				<view class="flex-1 px-2">余额支付</view>
				<!-- <image src="../../static/images/pay-icon1.png" class="wh34"></image> -->
				<image src="../../static/images/pay-icon2.png" class="wh34"></image>
			</view>
		</view>
		
		<view class="btn80 Mgb"
		@click="Router.navigateTo({route:{path:'/pages/deal-voucher/deal-voucher'}})">确定</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				Router:this.$Router,
				itemIndex:0
			}
		},
		methods: {
			
			changeItem(index){
				const self = this;
				self.itemIndex = index;
			},
			
		}
	}
</script>
<style>page{background-color: #f5f5f5;}</style>
<style scoped>
.py-6{padding-top: 60rpx;padding-bottom: 60rpx;}
input{font-size: 50rpx;flex: 1;}
.item{width: 160rpx;line-height: 70rpx;text-align: center;margin-bottom: 20rpx;margin-right: 20rpx;}
.item:nth-child(4n){margin-right: 0;}
.btn80{margin: 100rpx 20rpx 0;}
</style>
