<template>
	<view class="bT-e1">
		<view style="height:var(--status-bar-height)"></view>
		<view class="head flex1 pr-2 bB-e1 bg-white">
			<view class="px-2 py-3" @click="Router.back(1)">
				<image src="../../static/images/back.png" class="back"></image>
			</view>
			<view class="btn50-c Mgb">完成</view>
		</view>
		
		<view class="mx-2" v-show="type==0">
			<input type="text" value="" placeholder="输入昵称" placeholder-style="color:#222;"/>
			<view class="font-24 color9 py-2">好的昵称，会被别人更容易记住</view>
		</view>
		
		<view class="mx-2" v-show="type==1">
			<input type="text" value="" placeholder="输入你的姓名" placeholder-style="color:#222;"/>
			<view class="font-24 color9 py-2">为了保护您和他人的权益，请输入你的真实姓名</view>
		</view>
		
		<view class="mx-2" v-show="type==2">
			<input type="text" value="" placeholder="输入你的邮箱账号" placeholder-style="color:#222;"/>
			<view class="font-24 color9 py-2">为了保护您和他人的权益，请输入你的真实邮箱账号</view>
		</view>
		
		<view class="mx-2" v-show="type==3">
			<input type="text" value="" placeholder="输入你的身份证号" placeholder-style="color:#222;"/>
			<view class="font-24 color9 py-2">为了保护您和他人的权益，请输入你的真实身份证号</view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				Router:this.$Router,
				type:0
			}
		},
		onLoad(options) {
			const self = this;
			if(options){
				self.type = options.type;
			}
		},
		methods: {
			
		}
	}
</script>
<style>page{background-color: #fff;}</style>
<style scoped>
input{padding: 40rpx 0;border-bottom: 1px solid #e1e1e1;font-size: 28rpx;line-height: 1;}
.btn50-c{width: 110rpx;margin: 0;}
</style>
