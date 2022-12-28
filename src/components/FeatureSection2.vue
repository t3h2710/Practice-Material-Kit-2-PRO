<script setup>
import CardInfoFS2 from './CardInfoFS2.vue';
</script>
<template>
  <div class="margin_y_48 margin_x_75 padding_y_48 padding_x_24">

    <div class="flex_row ">
      <div class="width_half">
        
      </div>
      
      <div class="flex_row flex_wrap width_half">
        <CardInfoFS2
          class="width_half"
          :img="'/img/icon_info.png'"
          :word1="'Full Documentation'"
          :word2="'Built by developers for developers. Check the foundation and you will find everything inside our documentation.'"
        />
        <CardInfoFS2
          class="width_half"
          :img="'/img/icon_info.png'"
          :word1="'Bootstrap 5 Ready'"
          :word2="'The world’s most popular front-end open source toolkit, featuring Sass variables and mixins.'"
        />
        <CardInfoFS2
          class="width_half"
          :img="'/img/icon_info.png'"
          :word1="'Save Time & Money'"
          :word2="'Creating your design from scratch with dedicated designers can be very expensive. Start with our Design System.'"
        />
        <CardInfoFS2
          class="width_half"
          :img="'/img/icon_info.png'"
          :word1="'Fully Responsive'"
          :word2="'Regardless of the screen size, the website content will naturally fit the given resolution.'"
        />
      </div>
    </div>
 
  </div>
</template>
<style></style>