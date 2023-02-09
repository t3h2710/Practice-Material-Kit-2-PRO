<script setup>
import LogoMedia from './LogoMedia.vue';
</script>
<template>
  <div class="max_width_card margin_auto">
    <div class="flex_row flex_justify_center">
      <LogoMedia
      :img="'https://demos.creative-tim.com/material-kit-pro/assets/img/logos/gray-logos/logo-apple.svg'"
      />
      <LogoMedia
      :img="'https://demos.creative-tim.com/material-kit-pro/assets/img/logos/gray-logos/logo-facebook.svg'"
      />
      <LogoMedia
      :img="'https://demos.creative-tim.com/material-kit-pro/assets/img/logos/gray-logos/logo-nasa.svg'"
      />
      <LogoMedia
      :img="'https://demos.creative-tim.com/material-kit-pro/assets/img/logos/gray-logos/logo-vodafone.svg'"
      />
      <LogoMedia
      :img="'https://demos.creative-tim.com/material-kit-pro/assets/img/logos/gray-logos/logo-digitalocean.svg'"
      />
    </div>
  </div>
</template>