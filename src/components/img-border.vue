<template>
<image @click="handleClick" class="img-border" :src="str" ></image>
</template>
<script lang='ts'>

export default {
props:{
    str:String
},
methods:{
    handleClick(){
        console.log(123);
        this.$emit("srcChange",this.src)
    }
}

}
</script>
<style lang='scss'>
.img-border{
    border-radius: 50%;
}
</style>