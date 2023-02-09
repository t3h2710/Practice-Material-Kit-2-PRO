<template>
  <div class="flex_row gap_bt flex_justify_center padding_t_96 padding_b_48">
    <div>
      <h5 class="txt_darkgray fontsz_3 font_weight_6 line_height_4">Thank you for your support!</h5>
      <span class="txt_lightgray fontsz_2 font_weight_3 line_height_4">We deliver the best web products</span>
    </div>
    <div class="flex_row gap_10">
      <a href="">
        <Button 
          :bgColor="'bg_tweet'"
          :styleButton="'padding_y_15 padding_x_24 font_weight_3'"
          :iconLeft="'bi bi-twitter'"
        >
          TWEET
        </Button>
      </a>
      <a href="">
        <Button 
          :bgColor="'bg_fb'"
          :styleButton="'padding_y_15 padding_x_24 font_weight_3'"
          :iconLeft="'bi bi-facebook'"
        >
          SHARE
        </Button>
      </a>
      <a href="">
        <Button 
          :bgColor="'bg_pinterest'"
          :styleButton="'padding_y_15 padding_x_24 font_weight_3'"
          :iconLeft="'bi bi-pinterest'"
        >
          PIN IT
        </Button>
      </a>
   
    </div>

  </div>
</template>
<script setup>
import Button from './Button.vue';
</script>
