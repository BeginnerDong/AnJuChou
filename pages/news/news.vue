<template>
	<view>
		
		<view class="bg-white px-2">
			<view class="flex py-3 bB-e1" v-for="v in 2"
			@click="Router.navigateTo({route:{path:'/pages/newsDetail/newsDetail'}})">
				<image src="../../static/images/xiaoxi-img.png" class="img radius10"></image>
				<view class="pl-2 h150 py-1 flex5 flex-1">
					<view class="font-32 avoidOverflow2">公募基金资产净值合计17.69万亿元：权益基金成为最大推手 债基金</view>
					<view class="font-24 color9">2020.07.31</view>
				</view>
			</view>
			<view class="py-4 line-h">
				<view class="pb-3 font-32">绿城管理上半年收入8.15亿元，同比减少21.3%</view>
				<view class="font-24 color9">2020.07.31</view>
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
.img{width: 220rpx;height: 150rpx;}
.h150{height: 150rpx;}
</style>
