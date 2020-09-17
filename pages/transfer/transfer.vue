<template>
	<view>
		
		<view class="mt-2 px-2 py-4 bg-white line-h">
			<view class="d-flex a-end pb-3">
				<view class="font-34">招商泽瑞</view>
				<view class="font-30 pl-3">净值 <text class="colorR font-36">1.205</text></view>
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
		
		<view class="mt-2 bg-white px-3 py-4 line">
			<view class="flex1">
				<view class="font-32">调整转让价</view>
				<view class="count">
					<view class="countIcon"><image src="../../static/images/thetransfer-icon.png" class="countIcon1"></image></view>
					<view class="countNum">0.5%</view>
					<view class="countIcon"><image src="../../static/images/thetransfer-icon1.png" class="countIcon2"></image></view>
				</view>
			</view>
		</view>
		
		<view class="mt-2 bg-white px-2 py-4">
			<view class="color6 pb-5 line-1">转让金额</view>
			<view class="flex py-2 bB-f5">
				<view class="font-80">￥</view>
				<input type="number" value="" />
			</view>
			<view class="font-26 pt-3">投资不足6个月，转让需要收0.5%的手续费，满6个月无手续费。</view>
		</view>
		
		<view class="btn80 Mgb"
		@click="Router.navigateTo({route:{path:'/pages/deal-voucher/deal-voucher'}})">确定</view>
		
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

<style>
page{background-color: #f5f5f5;}
</style>

<style scoped>
.box{background-color: #f4f6fa;}
input{font-size: 80rpx;flex: 1;}
.btn80{margin: 100rpx 20rpx 0;}
</style>
