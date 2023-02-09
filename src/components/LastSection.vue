<template>
  <div class="last margin_t_30 max_width_card ">
    <div class="padding_y_48 flex_row gap_100 flex_align_center flex_justify_center">
      <div>
        <img style="width:40px" src="https://demos.creative-tim.com/material-kit-pro/assets/img/logo-ct-dark.png"
          alt="">
        <h5 class="txt_darkgray padding_y_20 fontsz_3 font_weight_5">Material Kit 2 PRO</h5>
        <div class="flex_row gap_20">
          <a href="https://www.facebook.com/CreativeTim/"><i class="bi bi-facebook txt_darkgray fontsz_2"></i></a>
          <a href="https://twitter.com/creativetim"><i class="bi bi-twitter txt_darkgray fontsz_2"></i></a>
          <a href="https://dribbble.com/creativetim"><i class="bi bi-dribbble txt_darkgray fontsz_2"></i></a>
          <a href="https://github.com/creativetimofficial"><i class="bi bi-github txt_darkgray fontsz_2"></i></a>
          <a href="https://www.youtube.com/channel/UCVyTG4sCw-rOvB9oHkzZD1w"><i class="bi bi-youtube txt_darkgray fontsz_2"></i></a>
        </div>
      </div>
      <div class="flex_row gap_70">
        <div v-for="item in list" >
          <h5 class="txt_darkgray line_height_6 font_weight_5 fontsz_1">{{ item.title }}</h5>
          <div class="flex_col">
            <span v-for="text in item.subTitle" class="txt_darkgray line_height_5">{{ text }}</span>
          </div>

        </div>
      </div>


    </div>
    <div class="txt_center padding_b_35">
      <span class="txt_darkgray">All rights reserved. Copyright © 2023 Material Kit by Creative Tim.</span>
    </div>
  </div>
</template>
<script setup>
defineProps({
  list: {
    type: Array,
    default: [],
  }
})
</script>
<style>
.last {
  margin-left: auto;
  margin-right: auto;
}
</style>