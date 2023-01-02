<template>
  <button 
    class="txt_white fontsz_a border_radius_5 padding_x_15 padding_y_10" 
    :class="bgColor"
  >
    <i :class="iconLeft"></i>
    <slot/>
    <i :class="iconRight"></i>
  </button>
</template>
<script setup>
defineProps({
  bgColor: {
    type: String,
    default: 'bg_primary',
  },
  iconLeft: {
    type: String,
  },
  iconRight: {
    type: String,
  },
})
</script>