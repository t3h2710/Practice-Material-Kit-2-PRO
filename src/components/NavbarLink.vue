<template>
  <a href="" class="flex_row flex_align_center txt_lightgray">
    <img id="imgL" class="icon" :src="imgLeft" @click="run" alt="">
    <span class="padding_x_10"><slot/></span>
    <img id="imgR" :src="imgRight" @click="walk" alt="">
  </a>
</template>

<script setup>
defineProps({
  imgLeft: {
    type: String,
  },
  imgRight: {
    type: String,
  },
})

function walk() {

}

function run() {

}

</script>
