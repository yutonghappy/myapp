<template>
  <view class="item">
    <img :src="Img"  class="item-img"/>
    <div class="item-content">
      <div class="item-name">
        Providence
      </div>
      <div class="item-score">
        807
      </div>
      <div class="item-desc">
        Seafood
      </div>
      <div class="item-btn">
        Find a table
      </div>
    </div>
    <div class="favor">
      <Follow width="24" height="24"></Follow>
    </div>
  </view>
</template>

<script setup lang="ts">

import Img from "@/assets/images/img1.jpg";
import { Follow } from '@nutui/icons-vue'
</script>

<style scoped lang="scss">
.item{
  height: 255px;
  width: 245px;
  margin-right: 10px;
  position: relative;
  .item-img{
    display: block;
    width: 100%;
    height: 150px;
    border-radius: 10px 10px 0 0;
  }
  display: inline-block;
  .item-content{
    background: #fff;
    width: 100%;
    display: flex;
    flex-direction: column;
    padding: 5px;
    box-sizing: border-box;
    height: 105px;
    border-radius: 0 0 10px 10px ;
    .item-name{
      font-weight: bold;
      font-size: 12px;
    }
    .item-score{
      font-size: 12px;
    }
    .item-desc{
      font-size: 12px;
    }
    .item-btn{
      width: 105px;
      height: 35px;
      background:#eeb236;
      border-radius: 35px;
      font-size: 12px;
      text-align: center;
      line-height: 35px;
    }
  }
  .favor{
    position: absolute;
    top: 10px;
    right: 5px;
    width: 40px;
    height: 40px;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #fff;
    border-radius: 50%;
  }
}
</style>
