<template>
  <div class="price_page bg_primary ">
    <div class="padding_y_48 flex_col flex_justify_center flex_align_center">
      <div class="max_width_txt_section txt_center">
        <Button class="margin_b_10 "
          :bgColor="'bg_bk'"
          :styleButton="'padding_y_5 padding_x_10'"
        >PRICING</Button>
        <h1 class="txt_white font_weight_6 fontsz_5 line_height_3">Ready to get Material Kit?</h1>
        <p class="txt_white line_height_3 font_weight_1 fontsz_2">Based on the license you get, you will have direct access to our team of developers who built the product.</p>
      
      </div>
      
    </div>
    <!-- <PriceCard class="margin_t_nagative1 padding_y_15">

    </PriceCard> -->
    <slot/>
  </div>
  
</template>
<script setup>
import Button from './Button.vue';

</script>
<style>
.price_page {
  background-image: linear-gradient(195deg,rgba(54, 157, 73, 0.5),rgba(4, 66, 16, 0.46)), url(https://demos.creative-tim.com/material-kit-pro/assets/img/shapes/pattern-lines.svg);
  height: 330px
}
</style>