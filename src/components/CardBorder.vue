<template>
  <div 
    class="card_common flex_row gap_20"
    :class="[COMPONENT_CARD_COLORS[bgColor], {
      'with_shadow': useShadow,
      'with_backdrop': backdrop,
    }]"
  >
    <div><i class="fontsz_3" :class="icon"></i><slot name="note"/></div>
    <div>
      <h4 class="fontsz_3 margin_b_10" :class="txtColor1"><slot name="title"/></h4>
      <div><i class="fontsz_3" :class="icon"></i><slot name="note"/></div>

      <p class="fontsz_1 line_height_3 font_weight_1 margin_b_20" :class="txtColor2"><slot name="decription"/></p>
      <span class="fontsz_1 font_weight_2" :class="txtColor3"><slot name="last"/></span>
    </div>
  </div>
</template>

<script setup>
import { COMPONENT_CARD_COLORS } from '../enums'


defineProps({
  bgColor: {
    type: String,
    default: 'default'
  },
  useShadow: {
    type: Boolean,
    default: true,
  },
  backdrop: {
    type: Boolean,
    default: false,
  },
  txtColor1: {
    type: String,
  },
  txtColor2: {
    type: String,
  },
  txtColor3: {
    type: String,
  },
  icon: {
    type: String,
  },
})
</script>

<style>
  .card_common {
    border-radius: 10px;
    padding: 20px;
  }
  .with_shadow {
    box-shadow: 0 2px 12px 0 rgb(0 0 0 / 16%);
  }
  .with_backdrop {
    backdrop-filter: saturate(200%) blur(30px);
  }
  
</style>
 <!-- :class="bgColor" -->
  <!-- :class="[bgColor, textColor]" -->
  <!-- :class="{ 'bg_primary': true / false }" -->
  <!-- :class="[bgColor, textColor, { 'bg_primary': true / false }]" -->

  <!-- colors = { main: 'value' } -->
  <!-- colors.main ==> value -->
  <!-- colors['main'] ==> value -->