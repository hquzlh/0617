<template>
	<view class="content">
		<view class="rpx">rpx</view>
		<view class="vw">vw</view>
		<view class="sass">sass</view>
	</view>
</template>

<script>
	export default {
		
	}
</script>

<style lang="scss">
	
	.rpx{
		width: 750rpx;
		height: 100px;
		background-color: aqua;
	}
	.vw{
		width: 50vw;
		height: 100px;
		background-color: tan;
	}
	.content{
		.sass{
			background-color: red;
		}
		color: $uni-color-primary;
	}
</style>
