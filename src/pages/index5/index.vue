<template>
	<view class="content">
		<img-border @srcChange="handleSrcChange" :str="src1"></img-border>
		<img-border @srcChange="handleSrcChange" :str="src2"></img-border>
		<view>
			子组件传递的数据:{{src}}
		</view>
	</view>
</template>

<script>
import { imgBorder } from "@/components/img-border";
	export default {
		data(){
			return {
				src:"",
				src1:"https://ss0.bdstatic.com/94oJfD_bAAcT8t7mm9GUKT-xh_/timg?image&quality=100&size=b4000_4000&sec=1592320987&di=b8eccfe26c9a9294009886672c7970c0&src=http://a3.att.hudong.com/14/75/01300000164186121366756803686.jpg",
				src2:"https://dss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=1906469856,4113625838&fm=26&gp=0.jpg"
			}
		},
		components:{
			imgBorder
		},
		methods:{
			handleSrcChange(e){
		
				this.src=e;
			}
		},
		onLoad(){
			console.log(this.baseUrl);
			console.log(getApp().globalData.base)
		}
	}
</script>

<style lang="scss">
	

</style>
