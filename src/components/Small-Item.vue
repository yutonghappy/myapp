<template>
  <view class="item">
    <img :src="Img"  class="item-img"/>
      <div class="item-name">
        Providence
      </div>
  </view>
</template>


<script lang="ts" setup>
import Img from "@/assets/images/img1.jpg";
</script>

<style lang="scss" scoped>
.item{
  display: inline-block;
  height: 125px;
  width: 120px;
  margin-right: 10px;
  .item-img{
    width: 100%;
    height: 85px;
    display: block;
    border-radius: 10px 10px 0 0;
  }

  .item-name{
    font-size: 12px;
    font-weight: bold;
    height: 40px;
    background: #fff;
    line-height: 40px;
    padding-left: 10px;
    border-radius: 0 0 10px 10px;
  }
}
</style>
