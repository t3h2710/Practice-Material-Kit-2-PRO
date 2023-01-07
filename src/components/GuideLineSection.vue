<script setup>
import CardBorder from './CardBorder.vue';

</script>
<template>
  <div class="max_width_card margin_auto">
    <div class="flex_row gap_20">
      <CardBorder
        :bgColor="'main'"
        :useShadow="false"
        :icon="'bi bi-flag-fill txt_white'"
        :txtColor1="'txt_white'"
        :txtColor2="'txt_white'"
        :txtColor3="'txt_white'"
      >
        <template #title>Getting Started</template>
        <template #decription>Check the possible ways of working with our product and the necessary files for building your own project.</template>
        <template #last>Let's start <i class="bi bi-arrow-right"></i></template>
      </CardBorder>

      <CardBorder
        :bgColor="'sub'"
        :useShadow="false"
        :icon="'bi bi-app txt_primary'"
        :txtColor1="'txt_darkgray'"
        :txtColor2="'txt_lightgray'"
        :txtColor3="'txt_primary'"
      >
        <template #title>Plugins</template>
        <template #decription>Get inspiration and have an overview about the plugins that we used to create the Material Kit.</template>
        <template #last>Read more <i class="bi bi-arrow-right"></i></template>
      </CardBorder>

      <CardBorder
        :bgColor="'sub'"
        :useShadow="false"
        :icon="'bi bi-arrow-through-heart-fill txt_primary'"
        :txtColor1="'txt_darkgray'"
        :txtColor2="'txt_lightgray'"
        :txtColor3="'txt_primary'"
      >
        <template #title>Utility Classes</template>
        <template #decription>Material Kit is giving you a lot of pre-made elements. For those who want flexibility, we included many utility classes.</template>
        <template #last>Read more <i class="bi bi-arrow-right"></i></template>
      </CardBorder>
      
    </div>

  </div>
</template>