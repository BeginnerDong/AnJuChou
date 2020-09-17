<template>
	<view>
		
		<view class="list mb-2">
			<view class="li" :class="liCurr==0?'on':''" @click="changeLi(0)">锁定</view>
			<view class="li" :class="liCurr==1?'on':''" @click="changeLi(1)">持有</view>
			<view class="li" :class="liCurr==2?'on':''" @click="changeLi(2)">转让</view>
			<view class="li" :class="liCurr==3?'on':''" @click="changeLi(3)">卖出</view>
		</view>
		
		<view class="bg-white px-3 mx-2 mt-2 radius10 line-h">
			<view class="font-24 color4 py-3 bB-e1 flex">
				<image src="../../static/images/investmentprojects-icon.png" class="wh28 mr-1"></image>
				<view>2020.08.23 购入时间</view>
			</view>
			<view>
				<view class="py-3">
					<view class="d-flex a-end flex-1 pb-2">
						<view class="font-32 font-w">招商泽瑞</view>
						<view class="pl-3">净值 <text class="colorR font-32 font-w">1.205</text></view>
					</view>
					<!-- 锁定 -->
					<view class="flex1 py-4 px-3 radius10 box" v-show="liCurr==0">
						<view class="font-24 color6">持有份额</view>
						<view class="font-32 colorM1 font-w">10000</view>
					</view>
					<!-- 其他 -->
					<view class="flex2 py-3  radius10 box" v-show="liCurr!=0">
						<view class="flex4">
							<view class="font-24 color6 pb-2">持有份额</view>
							<view class="font-32 colorM1 font-w">10000</view>
						</view>
						<view class="flex4">
							<view class="font-24 color6 pb-2">持有金额</view>
							<view class="font-32 colorM1 font-w">12050</view>
						</view>
						<view class="flex4">
							<view class="font-24 color6 pb-2">收益</view>
							<view class="font-32 colorM1 font-w">10000</view>
						</view>
					</view>
				</view>
				<view class="py-3 d-flex j-end bT-e1">
					<view class="btn60-M">撤回</view>
					<view class="btn60-M"
					@click="Router.navigateTo({route:{path:'/pages/sell/sell'}})">卖出</view>
					<view class="btn60 Mgb"
					@click="Router.navigateTo({route:{path:'/pages/transfer/transfer'}})">转让</view>
					<!-- <view class="btn60 Mgb"
					@click="Router.navigateTo({route:{path:'/pages/sell/sell'}})">修改</view> -->
				</view>
			</view>
		</view>
		
		<!-- 提醒弹框 -->
		<view class="bg-mask" v-show="is_show">
			<view class="mask p-aXY m-a text-c flex5">
				<view class="flex-1 flex4 line-h">
					<view class="font-w">现在不是项目卖出的开放时间</view>
					<view class="font-24 color6 pt-4">开放时间：每月1-5号</view>
				</view>
				<view class="font-26 bT-e1 flex font-w">
					<view class="w-50 py-4 bR-e1">我知道了</view>
					<view class="w-50 colorM py-4">去看看其他</view>
				</view>
			</view>
		</view>
		
		<!-- 撤回弹框 -->
		<view class="bg-mask" v-show="is_show1">
			<view class="mask p-aXY m-a text-c flex5">
				<view class="flex-1 flex4 line-h">你确定要撤回该项目的转让?</view>
				<view class="font-26 bT-e1 flex font-w">
					<view class="w-50 py-4 bR-e1">取消</view>
					<view class="w-50 colorM py-4">确认</view>
				</view>
			</view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				Router:this.$Router,
				liCurr:0,
				is_show:false,
				is_show1:false
			}
		},
		methods: {
			
			changeLi(i){
				const self = this;
				self.liCurr = i;
			},
			
		}
	}
</script>
<style>page{background-color: #f5f5f5;}</style>
<style scoped>
.li{width: 25%;font-size: 30rpx;padding: 40rpx 0;line-height: 1;}
.list{margin: 0;}
.list .on::before{width: 40rpx;height: 6rpx;border-radius: 3rpx;bottom: 0;left: 50%;margin-left: -20rpx;}

.box{background-color: #f4f6fa;}
.btn60-M{border-color: #e1e1e1;color: #666;width: 140rpx;margin: 0 0 0 30rpx;}
.btn60{width: 140rpx;margin: 0 0 0 30rpx;}

.mask{width: 620rpx;height: 320rpx;}
</style>
