<template>
  <button 
    class="fontsz_a border_radius_5" 
    :class="[bgColor, styleButton, txtColor]"
  >
    <i :class="iconLeft"></i>
    <slot/>
    <i :class="iconRight"></i>
  </button>
</template>
<script setup>
defineProps({
  txtColor: {
    type: String,
    default: 'txt_white'
  },
  bgColor: {
    type: String,
    default: 'bg_primary',
  },
  styleButton: {
    type: String,
    default: 'padding_x_15 padding_y_10',
  },
  iconLeft: {
    type: String,
  },
  iconRight: {
    type: String,
  },
})
</script>