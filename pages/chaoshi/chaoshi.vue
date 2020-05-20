<template>
	<view>
		<gridview :goods="goodsArr"></gridview>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				goodsArr: [{
						url: "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1589890900272&di=6ee2b249deef3cfc300edae184fd2832&imgtype=0&src=http%3A%2F%2Fimg.cnmo-img.com.cn%2F1722_600x1000%2F1721690.jpg",
						newprice: "12199",
						oldprice: "2499",
						title: "华为畅享10e4GB+64GB全网通版(幻夜黑)"
					},
					{
						url: "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1589890900272&di=6ee2b249deef3cfc300edae184fd2832&imgtype=0&src=http%3A%2F%2Fimg.cnmo-img.com.cn%2F1722_600x1000%2F1721690.jpg",
						newprice: "21993",
						oldprice: "2499",
						title: "华为畅享10e4GB+64GB全网通版(幻夜黑)"
					}, {
						url: "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1589890900272&di=6ee2b249deef3cfc300edae184fd2832&imgtype=0&src=http%3A%2F%2Fimg.cnmo-img.com.cn%2F1722_600x1000%2F1721690.jpg",
						newprice: "21992",
						oldprice: "2499",
						title: "华为畅享10e4GB+64GB全网通版(幻夜黑)"
					}, {
						url: "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1589890900272&di=6ee2b249deef3cfc300edae184fd2832&imgtype=0&src=http%3A%2F%2Fimg.cnmo-img.com.cn%2F1722_600x1000%2F1721690.jpg",
						newprice: "21996",
						oldprice: "2499",
						title: "华为畅享10e4GB+64GB全网通版(幻夜黑)"
					}, {
						url: "https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1589890900272&di=6ee2b249deef3cfc300edae184fd2832&imgtype=0&src=http%3A%2F%2Fimg.cnmo-img.com.cn%2F1722_600x1000%2F1721690.jpg",
						newprice: "2199",
						oldprice: "2499",
						title: "华为畅享10e4GB+64GB全网通版(幻夜黑)"
					}
				]
			}
		},
		onLoad() {

		},
		onPullDownRefresh() {
			setTimeout(() => {
				uni.stopPullDownRefresh()
				uni.showToast({
					title: '数据刷新完成',
					duration: 1000
				})
			}, 3000)
		},
		onReachBottom() {
			setTimeout(() => {
				uni.stopPullDownRefresh()
				uni.showToast({
					title: '数据刷新完成',
					duration: 1000
				})
			}, 1000)
		},
		methods: {

		}
	}
</script>

<style lang="scss">
</style>
