<template>
  <div 
    class="card_common flex_row gap_20 type1"
    :class="[COMPONENT_CARD_COLORS[bgColor], {
      'with_shadow': useShadow,
      'with_backdrop': backdrop,
    }]"
  >
  <!-- <div v-if="(position == 'right' || position == 'left')"><i class="fontsz_3" :class="icon"></i><slot name="note"/></div> -->
    <div v-if="(position == 'right')"><i class="fontsz_3 " :class="icon"></i>{{ note }}</div>
    <div>
      <h4 class="title fontsz_2 margin_b_10 line_height_1">{{ title }}</h4>
      <div class="icon_clock margin_b_20" v-if="(position == 'bottom')"><i class="fontsz_1" :class="icon"></i>{{ note }}</div>
      <p class="decription fontsz_1 line_height_3 font_weight_1 margin_b_20">{{ decription }}</p>
      <span v-if="last != null" class="last fontsz_1 font_weight_2" >{{ last }} <i :class="textIcon"></i></span>

      <span class="lastIcon" v-if="(lastIcon != null)" v-for="item in lastIcon">
        <i class="fontsz_1 font_weight_2 margin_r_5" :class="item"></i> 
      </span>
    </div>
  </div>
</template>

<script setup>
import { COMPONENT_CARD_COLORS } from '../enums'

defineProps({
  bgColor: {
    type: String,
    default: 'default'
  },
  useShadow: {
    type: Boolean,
    default: true,
  },
  backdrop: {
    type: Boolean,
    default: false,
  },
  note: {
    type: String,
  },
  title: {
    type: String,
  },
  decription: {
    type: String,
  },
  icon: {
    type: String,
  },
  position: {
    type: String,
  },
  last: {
    type: String,
  },
  textIcon: {
    type: String,
  },
  lastIcon: {
    type: Array,
  },
})
</script>

<style>
  .card_common {
    border-radius: 10px;
    padding: 20px;
    width: 33.33%;
  }
  .with_shadow {
    box-shadow: 0 2px 12px 0 rgb(0 0 0 / 16%);
  }
  .with_backdrop {
    backdrop-filter: saturate(200%) blur(30px);
  }
</style>
 <!-- :class="bgColor" -->
  <!-- :class="[bgColor, textColor]" -->
  <!-- :class="{ 'bg_primary': true / false }" -->

  <!-- :class="[bgColor, textColor, { 'bg_primary': true / false }]" -->

  <!-- colors = { main: 'value' } -->
  <!-- colors.main ==> value -->
  <!-- colors['main'] ==> value -->
  <!-- :class="percent > 0 ? 'text-success' : 'text-danger'" -->
  <!-- 
    :class="{
      'text-success': percent  >=  0 ,
      'text-danger': percent < 0,
    }" 
  -->
