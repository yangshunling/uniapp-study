<template>
	<view>
		<!-- 轮播图 -->
		<swiper class="swiper" :indicator-dots="indicatorDots" :autoplay="autoplay" :circular="true" :interval="interval"
		 :duration="duration">
			<swiper-item v-for="item in swiperArr" :key="item.id" style="width: 750rpx;height: 380rpx">
				<image :src="item" mode="scaleToFill" style="width: 100%;height: 100%;"></image>
			</swiper-item>
		</swiper>
		<!-- 导航栏 -->
		<view class="nav">
			<view class="nav_item">
				<view class="nav_view">
					<image class="nav_img" src="../../static/nav/chaoshi.png"></image>
				</view>
				<text class="nav_text">购物超市</text>
			</view>
			<view class="nav_item">
				<view class="nav_view">
					<image class="nav_img" src="../../static/nav/lianxi.png"></image>
				</view>
				<text class="nav_text">联系我们</text>
			</view>
			<view class="nav_item">
				<view class="nav_view">
					<image class="nav_img" src="../../static/nav/shequ.png"></image>
				</view>
				<text class="nav_text">社区图片</text>
			</view>
			<view class="nav_item">
				<view class="nav_view">
					<image class="nav_img" src="../../static/nav/shipin.png"></image>
				</view>
				<text class="nav_text"> 学习视频</text>
			</view>
		</view>
		<!-- 推荐商品 -->
		<view class="hot_goods">
			<view class="hot_title">推荐商品</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				swiperArr: [
					"https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1589878204001&di=f430293e4212b3887dfd452e0f5c545f&imgtype=0&src=http%3A%2F%2F01.minipic.eastday.com%2F20161229%2F20161229105231_a71df75a6b5be4281151b54b2bbd7362_4.jpeg",
					"https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1589878234820&di=4444c896ec59c401c2f168fce2f7cc5f&imgtype=0&src=http%3A%2F%2Fi0.hdslb.com%2Fbfs%2Farchive%2F839b48daee6bed189d49aa6eac912b353ce0db3d.jpg",
					"https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=2589661616,3622480363&fm=26&gp=0.jpg",
					"https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=186802938,579562787&fm=26&gp=0.jpg"
				],
				indicatorDots: true,
				autoplay: true,
				interval: 2000,
				duration: 500
			}
		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.nav {
		display: flex;
		margin: 20rpx 0rpx;

		.nav_item {
			display: flex;
			flex-direction: column;
			width: 25%;
			align-items: center;

			.nav_view {
				width: 80rpx;
				height: 80rpx;
				display: flex;
				justify-content: center;
				align-items: center;
				background: $app-main-color;
				border-radius: 60rpx;
				align-items: center;
				padding: 10rpx;

				.nav_img {
					width: 50rpx;
					height: 50rpx;
				}
			}

			.nav_text {
				font-size: 15px;
				padding-top: 10rpx;
			}
		}

	}

	.hot_goods {
		background: #eeeeee;
		overflow: hidden;
		.hot_title {
			font-size: 17px;
			color: $app-main-color;
			line-height: 40px;
			text-align: center;
			letter-spacing: 20px;
			background: $uni-bg-color;
			margin: 7rpx 0rpx;
		}
	}
</style>
