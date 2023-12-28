<template>
  <div class="page">
    <div class="header">
      <Horizontal />
      <ImageIcon></ImageIcon>
      <Search></Search>
    </div>
    <div class="action-bar">
      <div class="action-item">
        <MoreX />
        <span>Filter</span>
      </div>
      <div class="action-item">
        <Locationg3 />
        <span>Map</span>
      </div>
    </div>
    <div class="scrollX-box">
      <div class="scrollX-header">
        <div class="scrollX-header-title">Reserve a Table Online</div>
        <div class="scrollX-header-area"> See all </div>
      </div>
      <scroll-view :scroll-x="true" class="scrollX-content">
        <view class="scrollX-content-item">
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

        </view>
      </scroll-view>
    </div>
  </div>
</template>

<script lang="ts" setup>
import './index.scss'
import Img from '../../assets/images/img1.jpg'
import { Horizontal,Image as ImageIcon, Search,
  Locationg3,
  MoreX
} from '@nutui/icons-vue';
// import { Image } from '@nutui/nutui';
import { Image } from '@nutui/nutui';

</script>
