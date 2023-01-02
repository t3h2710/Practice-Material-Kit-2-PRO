<script setup>
import CardInfoFS2 from './CardInfoFS2.vue';
</script>
<template>
  <div class="margin_y_48 margin_x_75 padding_y_48 padding_x_95">

    <div class="flex_row flex_align_center ">
      <div class="width_half">
        <div class="card txt_center width_card_pink margin_auto">
          <div class="txt_white padding_b_96 padding_t_96 padding_x_16">
            <i class="bi bi-hand-index-fill" style="font-size: 25px"></i>
            <h3 class="font_weight_6 fontsz_4 margin_t_15">Feel the<br/>Material Kit</h3>
            <p class="fontsz_1 font_weight_1 line_height_4 margin_y_15">All the Bootstrap components that you need in a development have been re-design with the new look.</p>
          </div>
        </div>       
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

<style>
.card::before {
  content: '';
  display: block;
  border-radius: 0.5rem;
  background-image: -webkit-linear-gradient(90deg,rgba(236, 64, 122, 0.8) 0, rgba(216, 27, 96, 0.8) 180%), url('https://images.unsplash.com/photo-1569683795645-b62e50fbf103?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=987&q=80');
  background-position: center;
  background-size: cover;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  opacity: 1;
  z-index: -1;
}
.card {
  position: relative;
}
</style>