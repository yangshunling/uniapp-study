<template>
	<view class="news">
		<view class="news_item" v-for="(item,index) in newsArr" :key="index" @click="click_item(index)">
			<image class="img" :src="item.url"></image>
			<view class="right">
				<view class="top">
					{{item.title}}
				</view>
				<view class="bottom">
					<view class="time">
						发表时间：{{item.time}}
					</view>
					<view class="count">
						浏览：{{item.count}}
					</view>
				</view>
			</view>
		</view>

	</view>
</template>

<script>
	export default {
		data() {
			return {
				newsArr: [{
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}, {
					url: "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2348957240,2361878970&fm=26&gp=0.jpg",
					title: "百度图片使用世界前沿的人工智能技术",
					time: "20200520",
					count: "125"
				}]
			}
		},
		methods: {
			click_item(index) {
				uni.showToast({
					title: index.toString(),
					duration: 2000
				})
			}
		}
	}
</script>

<style lang="scss">
	.news {
		.news_item {
			padding: 15rpx;
			display: flex;
			border-bottom: 1px solid #B50E03;

			.img {
				width: 200rpx;
				margin-left: 10px;
				border-radius: 3px;
				height: 150rpx;
			}

			.right {
				margin: 0 10px;
				width: 550rpx;
				display: flex;
				flex-direction: column;
				justify-content: center;
			}

			.top {
				font-size: 17px;
			}

			.bottom {
				font-size: 13px;
				margin-top: 10px;
				display: flex;
				justify-content: space-between;
			}
		}
	}
</style>