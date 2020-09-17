<template>
	<view>
		
		<view class="d-flex a-end bg-white mt-2 py-4 px-2">
			<view class="font-34">招商泽瑞</view>
			<view class="font-30 pl-3">净值 <text class="colorR font-36">1.205</text></view>
		</view>
		
		<view class="px-2 bg-white mt-2 line-h bB-e1">
			<view class="flex1 py-6">
				<view class="font-34">买入金额</view>
				<view class="font-24 colorM"
				@click="Router.navigateTo({route:{path:'/pages/agreement/agreement'}})">《项目投资协议》</view>
			</view>
			<view class="flex py-4">
				<view class="font-80 font-w">￥</view>
				<input type="text" value="" placeholder="最低买入1000元" placeholder-style="color:#b7b7b7;font-size:32rpx;" />
			</view>
			<view class="flex flex-wrap pb-2">
				<view class="colorM b-e1 font-30 p-r item" 
				v-for="(item,index) in 4" :key="index" @click="changeItem(index)"
				:class="itemIndex==index?'borderM1 colorM1':''">
					<view>1万</view>
					<image src="../../static/images/pay-icon.png" class="wh34 p-a bottom-0 right-0" v-show="itemIndex==index"></image>
				</view>
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
input{font-size: 80rpx;flex: 1;}
.item{width: 160rpx;line-height: 70rpx;text-align: center;margin-bottom: 20rpx;margin-right: 20rpx;}
.item:nth-child(4n){margin-right: 0;}
.btn80{margin: 100rpx 20rpx 0;}
</style>
