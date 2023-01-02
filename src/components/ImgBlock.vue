<template>
  <div class="img_block margin_b_20">
    <div class="margin_b_10 padding_b_35 imgPage">
      <img class="width_full height_img" :src="imgUrl" alt="">
    </div>

    <h4 class="txt_darkgray fontsz font_weight_7 line_height_2 line_height_4 padding_x_10"><slot name="title"/></h4>
    <span class="txt_lightgray padding_x_10"><slot name="example"/></span>
  </div>
</template>

<style>
.imgPage {
  box-shadow: 0 2px 12px 0 rgb(0 0 0 / 16%);
  background-color: white;
  border-radius: 15px;
  overflow: hidden;
}
.height_img {
  height: 160px;
}
</style>
<script setup>
defineProps ({
  imgUrl: {
    type: String, 
    default: 'https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/sections/headers.jpg',
  },
  
})
</script>