<script setup>
</script>
<template>
  <div class="margin_y_75">
    <div class="centersection flex_col flex_align_center padding_16 margin_auto">
      <span class="txt_darkpink fontsz_a padding_x_10 padding_y_5 bg_light border_radius_5 font_weight_7 margin_y_20"><slot name="title"/></span>
      <h1 class="txt_darkgray font_weight_6 fontsz_5 line_height_2"><slot name="info"/></h1>
      <p class="txt_lightgray line_height_4 txt_center fontsz_3 font_weight_3"><slot name="description"/></p>
    </div>
  </div>
</template>
<style>
.centersection {
  max-width: 522px;
}
</style>