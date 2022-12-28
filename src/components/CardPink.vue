<template>
  <div 
    class="card_pink bg_primary"
    :class="{
      'with_shadow': useShadow
    }"
  >
    <slot/>
  </div>
</template>

<script setup>
defineProps({
  useShadow: {
    type: Boolean,
    default: true,
  }
})
</script>

<style>
.card_pink {
  border-radius: 10px;
}
.with_shadow {
  box-shadow: 0 2px 12px 0 rgb(0 0 0 / 16%);
}
</style>