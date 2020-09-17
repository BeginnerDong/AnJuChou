<template>
	<view>
		
		<view class="bg-f7 px-2 py-3 line-h">
			<picker mode="selector">
				<view class="font-32 color1 font-w pb-2 flex">
					<view>2020.08</view>
					<image src="../../static/images/project-icon.png" class="sj-icon ml-1"></image>
				</view>
			</picker>
			<view class="font-26 color8">
				<text class="pr-5">支出 ￥1,006.23</text>
				<text>收入 ￥1,006.23</text>
			</view>
		</view>
		
		<view class="d-flex a-start line-h px-2 pt-3">
			<image src="../../static/images/dealflow-icon.png" class="wh72"></image>     <!-- 充值 -->
			<!-- <image src="../../static/images/dealflow-icon2.png" class="wh72"></image> -->    <!-- 提现 -->
			<!-- <image src="../../static/images/dealflow-icon1.png" class="wh72"></image> -->    <!-- 卖出项目 -->
			<!-- <image src="../../static/images/dealflow-icon3.png" class="wh72"></image> -->    <!-- 转让项目 -->
			<!-- <image src="../../static/images/dealflow-icon4.png" class="wh72"></image> -->    <!-- 投资项目 -->
			<view class="pl-2 pt-1 bB-e1 pb-3 flex-1 flex1">
				<view>
					<view class="font-32 pb-2">充值</view>
					<view class="font-24 color8">今天 11:09</view>
				</view>
				<!-- <view class="font-36 font-w colorM1">+2.87</view> -->
				<view class="font-36 font-w">-522.87</view>
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

<style>
	page{background-color: #fff;}
.wh72{width: 72rpx;height: 72rpx;}
</style>
