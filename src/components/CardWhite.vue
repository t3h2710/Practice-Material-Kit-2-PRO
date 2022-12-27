<template>
  <div class="card_white">
    <slot/>
  </div>
</template>

<style>
  .card_white {
    background-color: rgba(255, 255, 255, 0.8);
    border-radius: 10px;
    box-shadow: 0 2px 12px 0 rgb(0 0 0 / 16%);
  }
</style>