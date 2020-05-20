<template>
	<view class="goods_list">
		<view class="goods_item" v-for="item in goods">
			<image mode="aspectFill" :src="item.url"></image>
			<view class="price">
				<text>￥{{item.newprice}}</text>
				<text>￥{{item.oldprice}}</text>
			</view>
			<view class="name"> {{item.title}} </view>
		</view>
	</view>
</template>

<script>
	export default {
		props: ["goods"],
		data() {
			return {

			};
		}
	}
</script>

<style lang="scss">
	.goods_list {
		padding: 0 15rpx;
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;

		.goods_item {
			width: 355rpx;
			margin-bottom: 10rpx;
			margin-top: 10rpx;
			background: #ffffff;
			box-sizing: border-box;
			border-radius: 5px;

			image {
				width: 100%;
				height: 350rpx;
				border-radius: 5px;
			}

			.price {
				color: $app-main-color;
				font-size: 36rpx;

				text:nth-child(2) {
					color: #ccc;
					font-size: 28rpx;
					margin-left: 10rpx;
					text-decoration: line-through;
				}
			}

			.name {
				font-size: 30rpx;
				line-height: 50rpx;
			}

			view {
				padding: 10rpx;
			}

		}
	}
</style>
