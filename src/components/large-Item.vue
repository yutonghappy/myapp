<template>
  <div class="item">
    <img :src="ImageItem" class="item-image"/>
    <div class="item-content">
        <div class="item-name">14.Russell's</div>
        <div  class="item-info">
          <div class="item-info-left">(431)</div>
          <div class="item-info-right">8mi</div>
        </div>
      <div  class="item-info">
        <div class="item-info-left">(431)</div>
        <div class="item-info-right">8mi</div>
      </div>
      <div class="item-desc">
        "during covid locked down was their Belgian waffle and
        breakfast burrito.
        "The food is delicious,the decor artsy"
      </div>
      <div class="item-btn"> Order online </div>
    </div>
  </div>
</template>


<script setup lang="ts">
import ImageItem from '@/assets/images/img1.jpg'

</script>


<style scoped lang="scss">
.item {
  margin-top: 10px;
  height: 335px;
  width: 100vw;
  &-image{
    height: 135px;
    width: 100%;
    display: block;
  }
  &-content {
    height: 200px;
    background: #fff;
    padding: 5px 10px;
    box-sizing: border-box;
    position: relative;
    .item-name{
      font-size: 14px;
      font-weight: bold;
    }
    .item-info {
      display: flex;
      justify-content: space-between;
      color: #6a6a6a;
      font-size: 12px;
    }
    .item-desc{
      font-size: 12px;
      color: #6a6a6a;
      margin-top: 10px;
    }
    .item-btn{
      display: inline-block;
      width: 105px;
      height: 35px;
      background:#eeb236;
      border-radius: 35px;
      font-size: 12px;
      text-align: center;
      line-height: 35px;
      position: absolute;
      bottom: 20px;
      right: 10px;
    }
  }
}
</style>
