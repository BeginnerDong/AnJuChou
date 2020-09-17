<template>
	<view>
		<view style="height:var(--status-bar-height)"></view>
		<view class="head flex1 pr-2 bB-e1 bg-white">
			<view class="px-2 py-3"
			@click="Router.back(1)">
				<image src="../../static/images/back.png" class="back"></image>
			</view>
			<view class="btn50-c Mgb">完成</view>
		</view>
		
		<view class="bg-white line-h px-2">
			<view class="flex bB-f5">
				<view class="py-4 txt">账号</view>
				<view class="font-30 ">15286589524</view>
			</view>
			<view class="flex">
				<view class="txt pt-6 pb-3">原密码</view>
				<input type="text" value="" placeholder="填写原密码" />
			</view>
			<view class="flex">
				<view class="txt pt-6 pb-3">新密码</view>
				<input type="text" value="" placeholder="填写新密码" />
			</view>
			<view class="flex">
				<view class="txt pt-6 pb-3">确认密码</view>
				<input type="text" value="" placeholder="填写再次确认密码" />
			</view>
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
<style>page{background-color: #f5f5f5;}</style>
<style scoped>
.btn50-c{width: 110rpx;margin: 0;}
.txt{width: 170rpx;}
.pt-6{padding-top: 60rpx;}
input{padding: 60rpx 0 30rpx;font-size: 28rpx;border-bottom: 1px solid #f5f5f5;flex: 1;}
</style>
