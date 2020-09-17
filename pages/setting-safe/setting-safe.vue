<template>
	<view>
		
		<view class="bg-white bT-e1 px-2 line-h font-30">
			<view class="flex1 py-4 bB-e1">
				<view class="flex-1">头像</view>
				<image src="../../static/images/my-icon.png" class="wh86 mr-3 radius-5"></image>
				<image src="../../static/images/thelogin-icon2.png" class="R-icon"></image>
			</view>
			<view class="flex1 py-4 bB-e1"
			@click="Router.navigateTo({route:{path:'/pages/setting-modify/setting-modify?type=0'}})">
				<view>昵称</view>
				<image src="../../static/images/thelogin-icon2.png" class="R-icon"></image>
			</view>
			<view class="flex1 py-4 bB-e1">
				<view>账号</view>
				<view>15682597458</view>
			</view>
			<view class="flex1 py-4"
			@click="Router.navigateTo({route:{path:'/pages/setting-password/setting-password'}})">
				<view>密码</view>
				<image src="../../static/images/thelogin-icon2.png" class="R-icon"></image>
			</view>
		</view>
		
		<view class="bg-white px-2 line-h font-30 mt-2">
			<view class="flex1 py-4 bB-e1"
			@click="Router.navigateTo({route:{path:'/pages/setting-modify/setting-modify?type=1'}})">
				<view>姓名</view>
				<view class="flex">
					<view></view>
					<image src="../../static/images/thelogin-icon2.png" class="R-icon ml-2"></image>
				</view>
			</view>
			<view class="flex1 py-4 bB-e1"
			@click="Router.navigateTo({route:{path:'/pages/setting-phone/setting-phone'}})">
				<view>手机号</view>
				<view class="flex">
					<view>18256849963</view>
					<image src="../../static/images/thelogin-icon2.png" class="R-icon ml-2"></image>
				</view>
			</view>
			<view class="flex1 py-4 bB-e1"
			@click="Router.navigateTo({route:{path:'/pages/setting-modify/setting-modify?type=2'}})">
				<view>绑定邮箱</view>
				<view class="flex">
					<view>未绑定</view>
					<image src="../../static/images/thelogin-icon2.png" class="R-icon ml-2"></image>
				</view>
			</view>
			<view class="flex1 py-4 bB-e1"
			@click="Router.navigateTo({route:{path:'/pages/setting-modify/setting-modify?type=3'}})">
				<view>身份证号</view>
				<view class="flex">
					<view>未绑定</view>
					<image src="../../static/images/thelogin-icon2.png" class="R-icon ml-2"></image>
				</view>
			</view>
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
<style>page{background-color: #f5f5f5;}</style>
<style scoped>
.wh86{width: 86rpx;height: 86rpx;}
.R-icon{width: 15rpx;}
</style>
