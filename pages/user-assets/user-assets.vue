<template>
	<view>
		
		<view class="m-3 p-r">
			<image src="../../static/images/assets-img.png" mode="widthFix"></image>
			<view class="p-aXY colorf line-h mt-4 px-4">
				<view class="font-26 pt-5 pb-2">总资产</view>
				<view class="font-60">420.00</view>
				<view class="flex1 pt-120">
					<view>
						<view class="font-26 pb-2">资产</view>
						<view class="font-32">20.00</view>
					</view>
					<view>
						<view class="font-26 pb-2">收益</view>
						<view class="font-32">20.00</view>
					</view>
					<view>
						<view class="font-26 pb-2">余额</view>
						<view class="font-32">20.00</view>
					</view>
				</view>
				<view class="flex0 p-a font-26 mx"
				@click="Router.navigateTo({route:{path:'/pages/user-assetsDetail/user-assetsDetail'}})">
					<image src="../../static/images/assets-icon.png" class="icon mr-1"></image>
					<view>资产明细</view>
				</view>
			</view>
		</view>
		
		<view class="px-2">
			<view class="btn80 Mgb"
			@click="Router.navigateTo({route:{path:'/pages/recharge/recharge'}})">充值</view>
			<view class="btn80-M"
			@click="Router.navigateTo({route:{path:'/pages/withdrawal/withdrawal'}})">提现</view>
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
.pt-120{padding-top: 100rpx;}
.btn80{margin-top: 200rpx;margin-bottom: 50rpx;}

.icon{width: 26rpx;height: 28rpx;}
.mx{background-color: #4868CC;width: 180rpx;height: 60rpx;border-radius: 30rpx 0 0 30rpx;top: 50rpx;right: 0;}
</style>
