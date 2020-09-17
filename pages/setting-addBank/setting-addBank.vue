<template>
	<view class="px-2">
		
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">姓名</view>
			<input type="text" value="" placeholder="请输入" />
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">电话</view>
			<input type="text" value="" placeholder="请输入" />
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">开户行</view>
			<input type="text" value="" placeholder="请输入" />
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">银行卡账号</view>
			<input type="text" value="" placeholder="请输入" />
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
<style>page{background-color: #fff;}</style>
<style scoped>
input{flex: 1;font-size: 26rpx;text-align: right;}
.Mgb{margin-top: 100rpx;}
</style>
