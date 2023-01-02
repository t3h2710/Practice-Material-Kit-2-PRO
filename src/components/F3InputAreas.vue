<script setup>
import ImgBlock from './ImgBlock.vue'
import WordBlock from './WordBlock.vue';
const titleImg = [
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/newsletters.jpg',
    title: 'Newsletters',
    example: '6 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/contact-sections.jpg',
    title: 'Contact Sections',
    example: '8 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/forms.jpg',
    title: 'Forms',
    example: '3 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/inputs.jpg',
    title: 'Inputs',
    example: '6 Examples',
  },
]
</script>
<template>
  <div class="">
    <div class="flex_row max_width_card margin_auto">
      <div class="width_quarter left_column">
        <WordBlock>
          <template #title>Input Areas</template>
          <template #description>50+ elements that you need for text manipulation and insertion</template>
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