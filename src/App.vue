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
import PresentationPages from './components/PresentationPages.vue'
import ComplexSection from './components/ComplexSection.vue'
import GuideLineSection from './components/GuideLineSection.vue'
import Pr from './components/Pr.vue'
import CX from './components/CX.vue'

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
      <PresentationPages></PresentationPages>
      <ComplexSection class="margin_t_48"></ComplexSection>
      <GuideLineSection class="margin_t_15"></GuideLineSection>
      <Pr></Pr>
      <CX></CX>


    
    </CardWhite>
  </div>
  

</template>
<style>
.bg {
  background-color: #eff1f5;
}
</style>