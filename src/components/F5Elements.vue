<script setup>
import ImgBlock from './ImgBlock.vue';
import WordBlock from './WordBlock.vue';
const titleImg = [
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/buttons.jpg',
    title: 'Buttons',
    example: '6 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/avatars.jpg',
    title: 'Avatars',
    example: '2 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/dropdowns.jpg',
    title: 'Dropdowns',
    example: '2 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/switch.jpg',
    title: 'Toggles',
    example: '2 Examples',
  },
  
]
</script>
<template>
  <div class="">
    <div class="flex_row max_width_card margin_auto">
      <div class="width_quarter left_column">
        <WordBlock>
          <template #title>Elements</template>
          <template #description>80+ carefully crafted small elements that come with multiple colors and shapes</template>
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
  <div class="space_bottom"></div>

</template>

<style>
.right_column > * {
  width: 33.33%;
  padding-left: 20px;
}
.right_column {
  width: 75%
}
.space_bottom {
  height: 200px;
}
</style>