<script setup>
import ImgBlock from './ImgBlock.vue'
import WordBlock from './WordBlock.vue';
const titleImg = [
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/navbars.jpg',
    title: 'Navbars',
    example: '4 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/nav-tabs.jpg',
    title: 'Nav Tabs',
    example: '2 Nav Tabs',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/pagination.jpg',
    title: 'Pagination',
    example: '3 Examples',
  },
]
</script>
<template>
  <div class="">
    <div class="flex_row max_width_card margin_auto">
      <div class="width_quarter left_column">
        <WordBlock>
          <template #title>Navigation</template>
          <template #description>30+ components that will help go through the pages</template>
        </WordBlock>
      </div>

      <div class="right_column flex_row flex_wrap ">
        <ImgBlock 
          v-for="item in titleImg"
          :imgUrl="item.pic"
        >
          <template #title>{{ item.title }}</template>
          <template #example>{{ item.example }}</template>
        </ImgBlock>
    
        
      </div>
    </div>
  </div>
</template>

<style>
.right_column > * {
  width: 33.33%;
  padding-left: 20px;
}
.right_column {
  width: 75%
}
</style>