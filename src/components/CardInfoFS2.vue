<template>
  <div class="">
    <div class="padding_y_20">
      <i class=" fontsz_3 font_weight_7 txt_primary" :class="icon"></i>
    </div>
    <h5 class="txt_darkgray fontsz_3 font_weight_7 line_height_2">{{ word1 }}</h5>
    <p class="txt_lightgray fontsz_1 font_weight_1 line_height_4 margin_r_90 margin_b_75 margin_t_15">{{ word2 }}</p>
</div>
  
</template>
<script setup>
defineProps({
  icon: {
    type: String
  },
  word1: {
    type: String
  },
  word2: {
    type: String
  },
})
</script>