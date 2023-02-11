<template>
  <Navbar>(CardWhite)(NavbarLink)(Button)</Navbar>
  <MainIntro></MainIntro>
    <div class="bg">
      <CardWhite class="margin_t_nagative margin_x_20">
        <FeatureSection1 class="margin_t_30">(CardNo)</FeatureSection1>
        <FeatureSection2>(CardInfoFS2)</FeatureSection2>
        <CollectionSection>(CenterSection)</CollectionSection>
        <DesignBlock>(ImgBlock)(WordBlock)</DesignBlock>
        <Navigation>(ImgBlock)(WordBlock)</Navigation>
        <InputAreas>(ImgBlock)(WordBlock)</InputAreas>
        <AttentionCatchers>(ImgBlock)(WordBlock)</AttentionCatchers>
        <Elements>(ImgBlock)(WordBlock)</Elements>
        <AccountSection>(Button)</AccountSection>
        <CodePageSection>(CenterSection)</CodePageSection>
        <PresentationPages>(ImgBlock)(WordBlock)</PresentationPages>
        <ComplexSection class="margin_t_48"></ComplexSection>
        <GuideLineSection class="margin_t_15">(CardBorder)</GuideLineSection>
        <Pr></Pr>
        <CX>(CardBorder)</CX>
        <MediaSection class="padding_y_48 margin_y_48">(LogoMedia)</MediaSection>
        <PriceSection>(Button)</PriceSection>
        <PriceCard class="margin_t_nagative" :list="priceCardList">(CardWhite, Button)</PriceCard>
        <Payment></Payment>
        <ThankSection>(Button)</ThankSection>
      </CardWhite>
      <LastSection :list="menuList"></LastSection>
    </div>
   
 
 </template>
 <!-- (Button)
 (CardBorder)
 (CardInfoFS2)
 (CardNo)	
 (CardPink)
 (CardWhite)
 (ImgBlock)
 (WordBlock)
 (LogoMedia) -->
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
import MediaSection from './components/MediaSection.vue'
import PriceSection from './components/PriceSection.vue'
import PriceCard from './components/PriceCard.vue'
import {priceCardList} from './components/data/data'
import Payment from './components/Payment.vue'
import ThankSection from './components/ThankSection.vue'
import LastSection from './components/LastSection.vue'
import { menuList } from './components/data/data'


</script>
 
 
 