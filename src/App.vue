<script setup>
import MainIntro from './components/MainIntro.vue'
import Navbar from './components/Navbar.vue'
import CardWhite from './components/CardWhite.vue'
import FeatureSection1 from './components/FeatureSection1.vue'
import FeatureSection2 from './components/FeatureSection2.vue'
import CollectionSection from './components/CollectionSection.vue'
import DesignBlock from './components/F1DesignBlock.vue'
import Navigation from './components/F2Navigation.vue'
import InputAreas from './components/F3InputAreas.vue'
import AttentionCatchers from './components/F4AttentionCatchers.vue'
import Elements from './components/F5Elements.vue'
import AccountSection from './components/AccountSection.vue'





import CodePageSection from './components/CodePageSection.vue'

</script>

<template>
  <Navbar></Navbar>
  <MainIntro></MainIntro>
  <div class="bg">
    <CardWhite class="margin_t_nagative margin_x_20">
      <FeatureSection1 class="margin_t_30"></FeatureSection1>
      <FeatureSection2></FeatureSection2>
      <CollectionSection></CollectionSection>
      <DesignBlock></DesignBlock>
      <Navigation></Navigation>
      <InputAreas></InputAreas>
      <AttentionCatchers></AttentionCatchers>
      <Elements></Elements>
      <AccountSection></AccountSection>
      <CodePageSection></CodePageSection>

    
    </CardWhite>
  </div>
  

</template>
<style>
.bg {
  background-color: #eff1f5;
}
</style>