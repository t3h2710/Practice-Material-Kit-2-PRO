<template>
  <div class="">
    <img class="margin_b_10 margin_t_15" :src="img" alt="" style="width: 40px">
    <h5 class="txt_darkgray fontsz_3 font_weight_7 line_height_2">{{ word1 }}</h5>
    <p class="txt_lightgray fontsz_1 font_weight_1 line_height_4 margin_r_90 margin_b_75 margin_t_15">{{ word2 }}</p>
</div>
  
</template>
<script setup>
defineProps({
  img: {
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