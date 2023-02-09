<template>
  <div class="width_one_fifth">
    <img :src="img" alt="" class="width_full">
  </div>
</template>
<script setup>
defineProps({
  img: {
    type: String,
  },
})
</script>