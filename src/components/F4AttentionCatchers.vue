<script setup>
import ImgBlock from './ImgBlock.vue'
import WordBlock from './WordBlock.vue';
const titleImg = [
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/alerts.jpg',
    title: 'Alerts',
    example: '4 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/toasts.jpg',
    title: 'Notifications',
    example: '3 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/popovers.jpg',
    title: 'Tooltips & Popovers',
    example: '2 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/modals.jpg',
    title: 'Modals',
    example: '5 Examples',
  },
]
</script>
<template>
  <div class="">
    <div class="flex_row max_width_card margin_auto">
      <div class="width_quarter left_column">
        <WordBlock>
          <template #title>Attention Catchers</template>
          <template #description>20+ Fully coded components that popup from different places of the screen</template>
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