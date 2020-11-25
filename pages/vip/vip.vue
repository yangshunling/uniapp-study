<template>
	<view>
		<button type="default" @click="start()">跳转到原生</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		methods: {
			start() {
				uni.sendNativeEvent("event", null)
			}
		}
	}
</script>

<style>

</style>
