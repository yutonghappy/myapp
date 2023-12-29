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
        <DefaultItem/>
        <DefaultItem/>
        <DefaultItem/>
        <DefaultItem/>
        <DefaultItem/>
      </scroll-view>
    </div>
    <div class="scrollX-box">
        <div class="scrollX-header">
          <div class="scrollX-header-title">
            Browse Los Angeles by Meal
          </div>
        </div>
      <scroll-view :scroll-x="true" class="scrollX-content">
        <SmallItem/>
        <SmallItem/>
        <SmallItem/>
        <SmallItem/>
      </scroll-view>
    </div>
    <LargeItem/>
  </div>
</template>

<script lang="ts" setup>
import './index.scss'
import Img from '../../assets/images/img1.jpg'
import { Horizontal,Image as ImageIcon, Search, Locationg3, MoreX } from '@nutui/icons-vue';
import SmallItem from "@/components/Small-Item.vue";
import DefaultItem from "@/components/default-Item.vue";
import LargeItem from "@/components/large-Item.vue";

</script>
