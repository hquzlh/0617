<template>
	<view class="content">
		<view data-index="1111"  @click="handleClick(1,$event)"> 
			点击我试试
		</view>
		<view  data-index="2222"  @click="handleClick(2,$event)"> 
			点击我试试222
		</view>
	</view>
</template>

<script>
	export default {
		methods:{
			handleClick(e,event){
				console.log(e);
				console.log(event.currentTarget.dataset.index);
			}
		}
	}
</script>

<style lang="scss">
	

</style>
