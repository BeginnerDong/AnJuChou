<template>
	<view>
		
		<view class="p-r">
			<!-- <view class="sign">进行中</view> -->
			<view class="sign bg90">已完成</view>
			<image src="../../static/images/home-img1.png" class="img"></image>
		</view>
		<!-- 进行中项目展示 -->
		<view>
			<view class="py-3 px-2 line-h">
				<view class="speed mb-2"></view>
				<view class="font-32 font-w flex1 pb-1 colorM1">
					<view>12,256.23</view>
					<view>21%</view>
				</view>
				<view class="flex1 font-24 color8">
					<view>目标200,000元</view>
					<view>筹款进度</view>
				</view>
			</view>
			<view class="h20-1"></view>
		</view>
		
		<view class="px-2 line-h">
			<view class="pt-4 pb-3 d-flex a-end">
				<view class="font-32 font-w">项目名称</view>
				<!-- 已完成项目展示 -->
				<!-- <view class="font-26 pl-3">当前净值 <text class="colorR font-28">1.523</text></view> -->
			</view>
			<!-- 进行中项目展示 -->
			<view class="flex font-30 color9">      
				距筹款结束
				<text class="timeTag">03</text>天
				<text class="timeTag">24</text>:
				<text class="timeTag">05</text>:
				<text class="timeTag">48</text>
			</view>
			<!-- 已完成项目展示 -->
			<!-- <view class="font-26 color9">
				筹款时间：2020.08.23-2020.08.30
			</view> -->
			
			<view class="flex2 py-5">
				<view class="flex4">
					<view class="font-36 font-w colorR">186,235.28</view>
					<view class="font-24 color8 pt-1">目前评估价</view>
				</view>
				<view class="flex4">
					<view class="font-36 font-w colorR">1.228</view>
					<view class="font-24 color8 pt-1">单位净值</view>
				</view>
			</view>
		</view>
		<view class="h20-1"></view>
		
		
		<!-- 已完成 -->
		<!-- <view>
			<view class="px-2 py-4 line-h">
				<view class="flex font-30 font-w">
					<image src="../../static/images/andproject-icon.png" class="wh42 mr-1"></image>
					<view>主要投资人信息</view>
				</view>
				<view class="py-4 bB-f5" v-for="(item,index) in 2" :key="index">
					<view class="font-36 pb-3">张 <text class="mh">丹</text></view>
					<view class="font-30 color8">投资额度：256325 <text class="mh">623588</text></view>
				</view>
			</view>
			<view class="h20-1"></view>
			<view class="px-2 pt-4 pb-2 line-h">
				<view class="flex font-30 font-w">
					<image src="../../static/images/andproject-icon1.png" class="wh42 mr-1"></image>
					<view>项目资料</view>
				</view>
				<view class="pt-4 flex flex-wrap">
					<view class="p-r photo" v-for="v in 4" @click="dataShow">
						<image src="../../static/images/andproject-img.png" class="wh220"></image>
						<view class="p-aX ">购房合同</view>
					</view>
				</view>
			</view>
			<view class="h20-1"></view>
		</view> -->
		
		
		<view class="px-2 py-4">
			<view class="flex pb-4 font-30 font-w">
				<image src="../../static/images/details-icon.png" class="wh42 mr-1"></image>
				<view>项目介绍</view>
			</view>
			<view>
				就白菜豆腐VB哦我割而郭敬明
			</view>
		</view>
		
		
		<!-- 进行时展示 -->
		<view>
			<view style="height: 120rpx;"></view>
			<view class="p-2 bT-f5 p-fX bottom-0 bg-white"
			@click="Router.navigateTo({route:{path:'/pages/buy/buy'}})">
				<view class="btn80 Mgb">立即投资</view>
			</view>
		</view>
		
		<!-- 权限弹框 -->
		<view class="bg-mask" v-show="is_show">
			<view class="mask p-aXY m-a text-c flex5">
				<view class="flex-1 flex4">很抱歉，您不是该项目的投资人，<br />无查看权限</view>
				<view class="font-26 py-4 bT-f5 color6">我知道了</view>
			</view>
		</view>
		
		<!-- 资料轮播 -->
		<view class="bg-mask px-5" v-show="data_show">
			<view class="p-aXY flex4">
				<swiper class="swiper-box mb-3" autoplay="autoplay" interval="3000" >
					<block>
						<swiper-item class="swiper-item" >
							<image src="../../static/images/andproject-img1.png" mode="widthFix" />
						</swiper-item>
					</block>
				</swiper>
				<image src="../../static/images/andproject-icon3.png" class="pageIcon l"></image>
				<image src="../../static/images/andproject-icon4.png" class="pageIcon r"></image>
				
				<image src="../../static/images/andproject-icon5.png" class="wh60 mt-5" @click="dataShow"></image>
			</view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				Router:this.$Router,
				is_show:false,
				data_show:false
			}
		},
		methods: {
			
			dataShow(){
				const self = this;
				self.data_show = !self.data_show;
			},
			
		}
	}
</script>
<style>
page{background-color: #fff;}
</style>
<style scoped>
.img{width: 100%;height: 320rpx;}
.sign{border-radius: initial;}
.bg90{background-color: #909090;}

.speed{width: 100%;height: 22rpx;border-radius: 11rpx;}
.speed::before{width: 21%;height: 22rpx;border-radius: 11rpx;}

.mh{filter: blur(8rpx);}

.photo{margin-right: 20rpx;margin-bottom: 20rpx;}
.photo:nth-child(3n){margin-right: 0;}
.photo view{background-color: rgba(0,0,0,0.5);line-height: 50rpx;text-align: center;color: #fff;font-size: 26rpx;bottom: 0;}

.mask{width: 620rpx;height: 320rpx;}

swiper,swiper-item{width: 600rpx;height: 750rpx;}
.pageIcon{width: 22rpx;height: 38rpx;position: absolute;top: 45%;}
.l{left: 20rpx;}
.r{right: 20rpx;}
</style>
