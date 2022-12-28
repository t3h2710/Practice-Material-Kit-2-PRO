<script setup>
import CardNo from './CardNo.vue'
</script>
<template>
<div class="feature1 flex_row gap_10 flex_align_center flex_justify_center width_FS margin_auto ">
  <CardNo >
    <template #number>300+</template>
    <template #tittle>Coded Elements</template>
    <template #description>From buttons, to inputs, navbars, alerts or cards, you are covered</template>
  </CardNo>
  <CardNo>
    <template #number>100+</template>
    <template #tittle>Design Blocks</template>
    <template #description>Mix the sections, change the colors and unleash your creativity</template>
  </CardNo>  
  <CardNo>
    <template #number>41</template>
    <template #tittle>Pages</template>
    <template #description>Save 3-4 weeks of work when you use our pre-made pages for your website</template>
  </CardNo>
</div>
</template>
<style>
.feature1 > * {
  width: 33.3333%;
}
</style>