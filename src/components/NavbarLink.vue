<template>
  <a href="" class="flex_row flex_align_center txt_lightgray">
    <img class="icon" :src="imgLeft" alt="">
    <slot/>
    <img :src="imgRight" alt="">
  </a>
</template>

<script setup>
defineProps({
  imgLeft: {
    type: String
  },
  imgRight: {
    type: String
  }
})
</script>
