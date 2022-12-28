<template>
  <div class="">
    <img class="margin_b_10" :src="img" alt="" style="width: 40px">
    <h5 class="txt_darkgray fontsz_3 font_weight_7 line_height_2">{{ word1 }}</h5>
    <p class="txt_lightgray fontsz_1 font_weight_3 line_height_3 margin_r_48 margin_b_48">{{ word2 }}</p>
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
  }
})
</script>