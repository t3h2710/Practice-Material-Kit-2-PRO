<script setup>
import MainIntro from './components/MainIntro.vue'
import Navbar from './components/Navbar.vue'
import CardWhite from './components/CardWhite.vue'
import FeatureSection1 from './components/FeatureSection1.vue'
import FeatureSection2 from './components/FeatureSection2.vue'

</script>

<template>
  <Navbar></Navbar>
  <MainIntro></MainIntro>
  <CardWhite class="margin_t_nagative padding_16 margin_x_20">
    <FeatureSection1 class="margin_t_30"></FeatureSection1>
    <FeatureSection2></FeatureSection2>
    
  </CardWhite>

</template>
<style>

</style>