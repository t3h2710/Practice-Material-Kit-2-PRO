<template>
  <div class="price_card max_width_card">
    <div class="flex_row flex_justify_center flex_align_stretch gap_20">
      <CardWhite
        class="width_quarter padding_y_20 padding_x_20"
        v-for="item in list"
      >
        <h5 class="title font_weight_6 line_height_4 fontsz_3">{{ item.title }}</h5>
        <p class="subtitle font_weight_1 line_height_3 ">{{ item.subTitle }}</p>
        <h3 class="price font_weight_6 fontsz_5 ">{{ item.price }}</h3>
        <Button 
          class="margin_b_48 width_full"
          v-bind="item">
          BUY NOW
        </Button>
        <p v-for="text in item.content">
          <i class="bi bi-check2 fontsz_3 icon_done"></i>
          <span class="txt_center font_weight_1 line_height_6 txt_content">{{ text }}</span> 
        </p>
      </CardWhite>
    </div>
  </div>
  



</template>
<script setup>
import CardWhite from './CardWhite.vue'
import Button from './Button.vue';

defineProps({
  list: {
    type: Array,
    default: [],
  }
})
</script>

<style>
.price_card {
  margin-left: auto;
  margin-right: auto;
}
/* .price_card .title {
  
} */
.price_card .subtitle {
  
}
.price_card .price {
  padding-top: 20px;
  padding-bottom: 30px;
}
.price_card .card_white:nth-child(1),
.price_card .card_white:nth-child(2),
.price_card .card_white:nth-child(4) {
  background: white;
}

.price_card .card_white:nth-child(3) {
  background: linear-gradient(1250deg,rgba(55, 55, 65, 0.9),rgba(17, 17, 17, 0.7)), #111;
}

.price_card .card_white:nth-child(1) .title,
.price_card .card_white:nth-child(2) .title,
.price_card .card_white:nth-child(4) .title {
  color: #344767

}
.price_card .card_white:nth-child(3) .title {
  color: white;

}
.price_card .card_white:nth-child(1) .subtitle,
.price_card .card_white:nth-child(2) .subtitle,
.price_card .card_white:nth-child(4) .subtitle {
  color: #344767

}
.price_card .card_white:nth-child(3) .subtitle {
  color: white;

}
.price_card .card_white:nth-child(1) .price,
.price_card .card_white:nth-child(2) .price,
.price_card .card_white:nth-child(4) .price {
  color: #344767

}
.price_card .card_white:nth-child(3) .price {
  color: white;

}
.price_card .card_white:nth-child(1) .icon_done,
.price_card .card_white:nth-child(2) .icon_done,
.price_card .card_white:nth-child(4) .icon_done {
  color: #344767;
  padding-right: 15px;

}
.price_card .card_white:nth-child(3) .icon_done {
  color: white;
  padding-right: 15px;


}
.price_card .card_white:nth-child(1) .txt_content,
.price_card .card_white:nth-child(2) .txt_content,
.price_card .card_white:nth-child(4) .txt_content {
  color: #344767

}
.price_card .card_white:nth-child(3) .txt_content {
  color: white;

}
/* .price_card .card_white:nth-child(1) {
  background: white;
}
.price_card .card_white:nth-child(2) {
  background: white;
}
.price_card .card_white:nth-child(3) {
  background: black;
}
.price_card .card_white:nth-child(4) {
  background: white;
} */

</style>