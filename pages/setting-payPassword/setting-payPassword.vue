<template>
	<view>
		<view style="height:var(--status-bar-height)"></view>
		<view class="head flex1 pr-2 bB-e1 bg-white">
			<view class="px-2 py-3"
			@click="Router.back(1)">
				<image src="../../static/images/back.png" class="back"></image>
			</view>
			<view class="pl-5 font-30">支付密码</view>
			<view class="btn50-c Mgb">完成</view>
		</view>
		
		<view class="flex1 pt-5 pb-3 bB-e1 mx-2">
			<view class="font-30">支付密码</view>
			<input type="text" value="" placeholder="请输入" />
		</view>
		<view class="flex1 pt-5 pb-3 bB-e1 mx-2">
			<view class="font-30">确认密码</view>
			<input type="text" value="" placeholder="请输入" />
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
input{flex: 1;font-size: 26rpx;text-align: right;}
.btn50-c{width: 110rpx;margin: 0;}
</style>
