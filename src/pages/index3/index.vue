<template>
	<view class="content">
		{{msg}}
		<view :data-color="color">color</view>
		<view>============</view>
		<view v-for="(item,index) in list" :key="item.id" v-if="item.id<=0" >{{item.id}}--{{item.test}}</view>
		<view> ￥{{money}}</view>
		<view>{{cnMoney}}</view>
		<view v-for="(item,index) in filterList" :key="item.id">{{item.id}}--{{item.test}}</view>
	</view>
</template>

<script>
	export default {
		data(){
			return{
				msg:"黑马程序员",
				color:"aqua",
				money:10000,
				list:[
					{
						id:0,
						test:"苹果"
					},
					{
						id:1,
						test:"香蕉"
					},
					{
						id:2,
						test:"樱桃"
					}
				]
			}
		},
		computed:{
			cnMoney(){
				return "￥"+this.money
			},
			filterList(){
				return this.list.filter(v=>v.id<=0);
			}
		}
	}
</script>

<style lang="scss">
	

</style>
