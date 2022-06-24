<template>
  <div>
    <!-- v-if  控制元素是否隐藏  直接删除该节点-->
    <!-- v-show  控制显示或者隐藏  频繁操作使用v-show 是给该元素设置一个style属性,并在style中添加display:node 隐藏属性-->
    <p v-show="bool">111111111111</p>
    <p v-show="booll">22222222222</p>
    <button @click="fn()">按钮</button>
  </div>
</template>

<script>
export default {
data(){
    return{
        bool:true,
        booll:false
    }
},
 methods:{
    fn(){
          this.bool=!this.bool;
          this.booll=!this.booll;
    }
 }
}
</script>

<style>

</style>