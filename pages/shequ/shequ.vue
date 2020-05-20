<template>
	<view class="root">
		<scroll-view class="left" :scroll-y="true">
			<view :class="selected==index?'active':''" v-for="(item,index) in leftArr" :key="index" @click="select_left(index)">{{item}}</view>
		</scroll-view>
		<view class="right">
			{{selected}}
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				leftArr: ["家具生活", "摄影设计", "明星美女", "空间设计", "户型装饰", "摄影学习", "摄影设计", "明星美女", "空间设计", "户型装饰", "摄影学习", "家具生活", "摄影设计",
					"明星美女", "空间设计", "户型装饰", "摄影学习", "摄影设计", "明星美女", "空间设计", "户型装饰", "摄影学习"
				],
				selected: 0
			}
		},
		methods: {
			select_left(index) {
				this.selected = index;
				console.log(this.selected)
			}
		}
	}
</script>

<style lang="scss">
	page {
		height: 100%
	}

	.root {
		height: 100%;
		display: flex;

		.left {
			width: 200rpx;
			height: 100%;
			border-right: 1rpx solid #eee;

			view {
				line-height: 100rpx;
				text-align: center;
				font-size: 15px;
				border-bottom: 1rpx solid #eee;
			}

			.active {
				background: $app-main-color;
				color: #fff;
			}

		}

		.right {
			width: 550rpx;
			height: 100%;
			text-align: center;
		}
	}
</style>
