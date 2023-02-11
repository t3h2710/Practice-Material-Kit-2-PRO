<script setup>
import CardBorder from './CardBorder.vue';
import {menuinGuideLine} from './data/data'

</script>
<template>
  <div class="guideLine max_width_card margin_auto">
    <div class="flex_row gap_20">
      <CardBorder
        v-for="item in menuinGuideLine"
          :bgColor="item.bgColor"
          :useShadow="item.useShadow"
          :position="item.position"
          :icon="item.icon"
          :title="item.title"
          :decription="item.decription"
          :last="item.last"
          :textIcon="item.textIcon"
      >
      </CardBorder>
    </div>

  </div>
</template>
<style>
.guideLine .card_common:nth-child(2) .title,
.guideLine .card_common:nth-child(3) .title {
  color: var(--text_dark_gray)
}
.guideLine .card_common:nth-child(1) .title {
  color: var(--text_w)

}
.guideLine .card_common:nth-child(2) .icon_clock,
.guideLine .card_common:nth-child(3) .icon_clock {
  color: var(--text_light_gray)
}
.guideLine .card_common:nth-child(1) .icon_clock {
  color: var(--text_w)
}

.guideLine .card_common:nth-child(2) .decription,
.guideLine .card_common:nth-child(3) .decription {
  color: var(--text_light_gray)
}
.guideLine .card_common:nth-child(1) .decription {
  color: var(--text_w)
}

.guideLine .card_common:nth-child(2) .last,
.guideLine .card_common:nth-child(3) .last {
  color: var(--text_primary_color)
}
.guideLine .card_common:nth-child(1) .last {
  color: var(--text_w)
}
</style>