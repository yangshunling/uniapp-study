<template>
	<view>
		<web-view :webview-styles="webviewStyles" src="https://blog.csdn.net/u014752325/article/details/107605689"></web-view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				webviewStyles: {
					progress: {
						color: '#FF3333'
					}
				}
			}
		},
		methods: {

		}
	}
</script>

<style>

</style>
