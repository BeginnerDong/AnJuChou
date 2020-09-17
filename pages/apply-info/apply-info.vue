<template>
	<view class="px-2 line-h">
		
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">姓名</view>
			<input type="text" value="" placeholder="请输入" />
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">电话</view>
			<input type="text" value="" placeholder="请输入" />
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">婚姻状况</view>
			<view class="flex font-26">
				<view class="flex pr-5">
					<image src="../../static/images/toapplyfor-icon1.png" class="wh32 mr-1"></image>
					<!-- <image src="../../static/images/toapplyfor-icon.png" class="wh32 mr-1"></image> -->
					<view>未婚</view>
				</view>
				<view class="flex">
					<!-- <image src="../../static/images/toapplyfor-icon1.png" class="wh32 mr-1"></image> -->
					<image src="../../static/images/toapplyfor-icon.png" class="wh32 mr-1"></image>
					<view>已婚</view>
				</view>
			</view>
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">学历</view>
			<picker mode="selector">
				<view class="font-26 color9 flex-1 flex">
					<view>请选择</view>
					<image src="../../static/images/thelogin-icon2.png" class="R-icon ml-1"></image>
				</view>
			</picker>
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">学位</view>
			<picker mode="selector">
				<view class="font-26 color9 flex-1 flex">
					<view>请选择</view>
					<image src="../../static/images/thelogin-icon2.png" class="R-icon ml-1"></image>
				</view>
			</picker>
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">工作单位</view>
			<input type="text" value="" placeholder="请输入" />
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">职位</view>
			<picker mode="selector">
				<view class="font-26 color9 flex-1 flex">
					<view>请选择</view>
					<image src="../../static/images/thelogin-icon2.png" class="R-icon ml-1"></image>
				</view>
			</picker>
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">工作年限</view>
			<picker mode="selector">
				<view class="font-26 color9 flex-1 flex">
					<view>请选择</view>
					<image src="../../static/images/thelogin-icon2.png" class="R-icon ml-1"></image>
				</view>
			</picker>
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">公积金年限</view>
			<picker mode="selector">
				<view class="font-26 color9 flex-1 flex">
					<view>请选择</view>
					<image src="../../static/images/thelogin-icon2.png" class="R-icon ml-1"></image>
				</view>
			</picker>
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">社保年限</view>
			<picker mode="selector">
				<view class="font-26 color9 flex-1 flex">
					<view>请选择</view>
					<image src="../../static/images/thelogin-icon2.png" class="R-icon ml-1"></image>
				</view>
			</picker>
		</view>
		<view class="flex1 py-4 bB-e1">
			<view class="font-30">年收入</view>
			<picker mode="selector">
				<view class="font-26 color9 flex-1 flex">
					<view>请选择</view>
					<image src="../../static/images/thelogin-icon2.png" class="R-icon ml-1"></image>
				</view>
			</picker>
		</view>
		<view class="py-4 bB-e1">
			<view class="font-30 pb-3">筹款说明</view>
			<textarea value="" placeholder="请输入" />
		</view>
		<view class="font-24 py-2 line-h pb-5">申请之后，平台收到信息后会人工回访，跟进</view>
		
		
		<view style="height: 130rpx;"></view>
		<view class="bg-white p-2 p-fX bottom-0 shadowT">
			<view class="btn80 Mgb"
			@click="Router.navigateTo({route:{path:'/pages/apply-finish/apply-finish'}})">确定申请</view>
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
textarea{width: 100%;height: 220rpx;background-color: #f5f5f5;font-size: 26rpx;padding: 20rpx;box-sizing: border-box;}
</style>
