<script setup>
import CardBorder from './CardBorder.vue';
import {menuinCX} from './data/data'

</script>
<template>
  <div class="cx max_width_card margin_auto">
    <div  class="flex_row gap_20">
      <CardBorder
        v-for="item in menuinCX"
          :bgColor="item.bgColor"
          :useShadow="item.useShadow"
          :position="item.position"
          :icon="item.icon"
          :note="item.note"
          :title="item.title"
          :decription="item.decription"
          :lastIcon="item.lastIcon"
      >
      
      </CardBorder>
      
      
    </div>

  </div>
</template>
<style>
.cx {

}
/* .cx .card_common:nth-child(1),
.cx .card_common:nth-child(3) {
  background: var();
}
.cx .card_common:nth-child(2) {
} */
.cx .card_common:nth-child(1) .title,
.cx .card_common:nth-child(3) .title {
  color: var(--text_dark_gray)
}
.cx .card_common:nth-child(2) .title {
  color: var(--text_w)

}
.cx .card_common:nth-child(1) .icon_clock,
.cx .card_common:nth-child(3) .icon_clock {
  color: var(--text_light_gray)
}
.cx .card_common:nth-child(2) .icon_clock {
  color: var(--text_w)
}

.cx .card_common:nth-child(1) .decription,
.cx .card_common:nth-child(3) .decription {
  color: var(--text_light_gray)
}
.cx .card_common:nth-child(2) .decription {
  color: var(--text_w)
}

.cx .card_common:nth-child(1) .lastIcon,
.cx .card_common:nth-child(3) .lastIcon {
  color: var(--text_light_gray)
}
.cx .card_common:nth-child(2) .lastIcon {
  color: var(--text_w)
}


</style>