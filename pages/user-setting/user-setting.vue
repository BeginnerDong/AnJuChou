<template>
	<view>
		
		<view class="bg-white bT-e1 px-2 line-h">
			<view class="flex1 py-4 bB-e1"
			@click="Router.navigateTo({route:{path:'/pages/setting-safe/setting-safe'}})">
				<view>账户与安全</view>
				<image src="../../static/images/thelogin-icon2.png" class="R-icon"></image>
			</view>
			<view class="flex1 py-4 bB-e1"
			@click="Router.navigateTo({route:{path:'/pages/setting-bank/setting-bank'}})">
				<view>银行卡管理</view>
				<image src="../../static/images/thelogin-icon2.png" class="R-icon"></image>
			</view>
			<view class="flex1 py-4 bB-e1"
			@click="Router.navigateTo({route:{path:'/pages/setting-payPassword/setting-payPassword'}})">
				<view>交易密码</view>
				<image src="../../static/images/thelogin-icon2.png" class="R-icon"></image>
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

<style>
page{background-color: #f5f5f5;}
</style>
