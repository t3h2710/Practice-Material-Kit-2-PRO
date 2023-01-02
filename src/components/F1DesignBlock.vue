<script setup>
import ImgBlock from './ImgBlock.vue'
import WordBlock from './WordBlock.vue'

const titleImg = [
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/headers.jpg',
    title:'Page Header', 
    example: '10 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/features.jpg',
    title:'Features', 
    example: '14 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/pricing.jpg',
    title:'Pricing', 
    example: '8 Examples',
  },
  {
    pic:'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/faq.jpg',
    title:'FAQ', 
    example: '1 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/blogs.jpg',
    title:'Blog Posts', 
    example: '11 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/testimonials.jpg',
    title:'Testimonials', 
    example: '11 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/teams.jpg',
    title:'Teams', 
    example: '6 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/stats.jpg',
    title:'Stats', 
    example: '3 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/call-to-action.jpg',
    title:'Call to Actions', 
    example: '8 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/projects.jpg',
    title:'Applications', 
    example: '6 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/logo-area.jpg',
    title:'Logo Areas', 
    example: '4 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/footers.jpg',
    title:'Footers', 
    example: '10 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/general-cards.jpg',
    title:'General Cards', 
    example: '9 Examples',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/content-sections.jpg',
    title:'Content Sections', 
    example: '8 Examples',
  },

]

</script>

<template>
  <div class="">
    <div class="flex_row max_width_card margin_auto">
      <div class="width_quarter left_column">
        <WordBlock>
          <template #title>Design Blocks</template>
          <template #description>A selection of 45 page sections that fit perfectly in any combination</template>
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
  width: 75%;
}

</style>