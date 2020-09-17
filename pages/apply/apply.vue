<template>
	<view>
		
		<view class="bg-white px-2 mt-2 pb-3">
			<view class="flex font-24 color4 py-3 line-h bB-e1">
				<image src="../../static/images/investmentprojects-icon.png" class="wh28"></image>
				<view class="px-1">2020.08.23</view>
				<view>申请时间</view>
			</view>
			<view class="pt-3 avoidOverflow3">
				hi顾服务IE染发博文为认同感奇偶为人体hi顾服务IE染发博文为认同感奇偶为人体hi顾服务IE染发博文为认同感奇偶为人体hi顾服务IE染发博文为认同感奇偶为人体hi顾服务IE染发博文为认同感奇偶为人体hi顾服务IE染发博文为认同感奇偶为人体hi顾服务IE染发博文为认同感奇偶为人体hi顾服务IE染发博文为认同感奇偶为人体hi顾服务IE染发博文为认同感奇偶为人体
			</view>
		</view>
		
		<view style="height: 150rpx;"></view>
		<view class="p-2 p-fX bottom-0">
			<view class="font-26 color9 text-c line-h pb-2">推荐10个用户可申请一次筹款</view>
			<view class="btn80 Mgb"
			@click="Router.navigateTo({route:{path:'/pages/apply-info/apply-info'}})">去申请</view>
		</view>
		
		
		<!-- 推荐未达标弹框 -->
		<view class="bg-mask" v-show="is_show">
			<view class="mask p-aXY">
				<view class="txt">很抱歉，您推荐的用户还未达到10个用户</view>
				<view class="btn70 Mgb">去推荐</view>
				<image src="../../static/images/toapplyfor-icon2.png" class="wh20 m-2 p-a top-0 right-0"></image>
			</view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				Router:this.$Router,
				is_show:false
			}
		},
		methods: {
			
		}
	}
</script>
<style>
page{background-color: #f5f5f5;}
</style>
<style scoped>

.mask{width: 620rpx;height: 442rpx;}
.mask .txt{width: 400rpx;text-align: center;padding: 110rpx 0;margin: auto;}
.btn70{width: 200rpx;}
</style>
