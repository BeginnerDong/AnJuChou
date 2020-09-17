<template>
	<view class="bT-e1">
		
		<view class="mx-2 p-3 mt-4 shadow radius10 line-h">
			<view class="flex">
				<image src="../../static/images/bankcard-icon.png" class="wh70"></image>
				<view class="pl-2 font-w">
					<view class="font-24 pb-2">中国银行</view>
					<view class="font-30">**** **** **** 2356</view>
				</view>
			</view>
			<view class="flex1 pt-4">
				<view class="flex">
					<image src="../../static/images/bankcard-icon1.png" class="wh32 mr-1"></image>
					<!-- <image src="../../static/images/pay-icon2.png" class="wh32 mr-1"></image> -->
					<view class="font-22 color6">默认银行卡</view>
				</view>
				<view class="flex font-24 color9">
					<view class="flex px-3">
						<image src="../../static/images/bankcard-icon2.png" class="wh24 mr-1"></image>
						<view>编辑</view>
					</view>
					<view class="flex pl-3">
						<image src="../../static/images/bankcard-icon3.png" class="wh24 mr-1"></image>
						<view>删除</view>
					</view>
				</view>
			</view>
		</view>
		
		
		<view style="height: 140rpx;"></view>
		<view class="p-2 bg-white bT-e1 p-fX bottom-0">
			<view class="btn80 Mgb"
			@click="Router.navigateTo({route:{path:'/pages/setting-addBank/setting-addBank'}})">添加银行卡</view>
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

<style>
page{background-color: #fff;}
</style>
