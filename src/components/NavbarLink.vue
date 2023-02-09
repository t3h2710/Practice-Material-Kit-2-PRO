<template>
  <a href="" class="flex_row flex_align_center txt_lightgray">
    <i class="icon" :class="iconLeft"></i>
    <!-- <img id="imgL" class="icon" :src="imgLeft" @click="run" alt=""> -->
    <span class="padding_x_10"><slot/></span>
    <i :class="iconRight"></i>
    <!-- <img id="imgR" :src="iconRight" @click="walk" alt=""> -->
  </a>
</template>

<script setup>
defineProps({
  iconLeft: {
    type: String,
  },
  iconRight: {
    type: String,
  },
})

function walk() {

}

function run() {

}

</script>
