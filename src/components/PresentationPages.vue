<script setup>
import ImgBlock from './ImgBlock.vue';
import WordBlock from './WordBlock.vue';
const titleImg = [
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/pages/coworking.jpg',
    title: 'Coworking Page',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/pages/rental.jpg',
    title: 'Rental Page',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/pages/case-study.jpg',
    title: 'Case Study',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/pages/about-us.jpg',
    title: 'About Us Page',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/pages/pricing.jpg',
    title: 'Pricing Page',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/pages/career.jpg',
    title: 'Career Page',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/pages/work-with-us.jpg',
    title: 'Work With Us',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/pages/terms.jpg',
    title: 'Terms & Conditions',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/pages/help-center.jpg',
    title: 'Help Center',
  },
  {
    pic: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/pages/help-center-basic.jpg',
    title: 'Help Center Basic',
  },
  
]
</script>
<template>
  <div class="flex_row max_width_card margin_auto">
    <div class="flex_row flex_wrap width_three_quarter">
      <ImgBlock
      class="width_one_third padding_r_20"
        v-for="item in titleImg"
        :imgUrl="item.pic"
      >
        <template #title>{{ item.title }}</template>
      </ImgBlock>
    </div>
    <div class="width_quarter margin_l_50">
      <WordBlock>
        <template #title>Presentation Pages for Company, Landing Pages, Blogs and Support</template>
        <template #description>These is just a small selection of the multiple possibitilies you have. Focus on the business, not on the design.</template>
      </WordBlock>
    </div>
  </div>
</template>