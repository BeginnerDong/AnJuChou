<template>
	<view>
		
		<!-- <view class="py-3 text-c colorM1 font-30 bg-f5 line-h">
			申请中
		</view> -->
		<view class="py-3 colorM1 font-30 bg-f5 line-h flex1 px-2">
			<view>申请不通过</view>
			<view class="font-24 color9 flex-1 d-flex j-end a-center"
			@click="Router.navigateTo({route:{path:'/pages/apply-reason/apply-reason'}})">
				<view>请选择</view>
				<image src="../../static/images/thelogin-icon2.png" class="R-icon ml-1"></image>
			</view>
		</view>
		
		<view class="flex1 pt-5 pb-3 mx-2 bB-e1">
			<view class="font-30">姓名</view>
			<view>张丹</view>
		</view>
		<view class="flex1 pt-5 pb-3 mx-2 bB-e1">
			<view class="font-30">电话</view>
			<view>张丹</view>
		</view>
		<view class="flex1 pt-5 pb-3 mx-2 bB-e1">
			<view class="font-30">婚姻状况</view>
			<view class="flex font-26">
				<image src="../../static/images/toapplyfor-icon1.png" class="wh32 mr-1"></image>
				<!-- <image src="../../static/images/toapplyfor-icon.png" class="wh32 mr-1"></image> -->
				<view>未婚</view>
			</view>
		</view>
		<view class="flex1 pt-5 pb-3 mx-2 bB-e1">
			<view class="font-30">学历</view>
			<view>张丹</view>
		</view>
		<view class="flex1 pt-5 pb-3 mx-2 bB-e1">
			<view class="font-30">学位</view>
			<view>张丹</view>
		</view>
		<view class="flex1 pt-5 pb-3 mx-2 bB-e1">
			<view class="font-30">工作单位</view>
			<view>张丹</view>
		</view>
		<view class="flex1 pt-5 pb-3 mx-2 bB-e1">
			<view class="font-30">职位</view>
			<view>张丹</view>
		</view>
		<view class="flex1 pt-5 pb-3 mx-2 bB-e1">
			<view class="font-30">工作年限</view>
			<view>张丹</view>
		</view>
		<view class="flex1 pt-5 pb-3 mx-2 bB-e1">
			<view class="font-30">公积金年限</view>
			<view>张丹</view>
		</view>
		<view class="flex1 pt-5 pb-3 mx-2 bB-e1">
			<view class="font-30">社保年限</view>
			<view>张丹</view>
		</view>
		<view class="flex1 pt-5 pb-3 mx-2 bB-e1">
			<view class="font-30">年收入</view>
			<view>张丹</view>
		</view>
		<view class="py-5 mx-2">
			<view class="font-30 pb-3">筹款说明</view>
			<view class="p-3 bg-f5">张丹</view>
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
