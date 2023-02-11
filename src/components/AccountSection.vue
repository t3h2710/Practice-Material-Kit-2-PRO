<script setup>
import Button from './Button.vue';
import {accountSImg} from './data/data'
</script>
<template>
  <div class="account_page flex_justify_center flex">
    <div class="flex_row max_width_card ">
      <div class="width_quarter left_col flex_col flex_justify_center">
        <h2 class="txt_white fontsz_4 font_weight_7 line_height_2 margin_b_20">Account Pages for beautiful webapps</h2>
        <span class="line_height_2 margin_b_20 fontsz_1 font_weight_1 txt_p">We created many examples for pages like Signup, Signin, Forgot Password, 2FA Authentification and so on. Just choose between a Basic Design, an illustration or a cover and you are good to go!</span>
        <div>
          <Button>VIEW PAGES</Button>
          <Button :bg-color="'bg_transparent'">VIEW SIGNUP PAGES</Button>
        </div>
        
      </div>
      <div class="width_three_quarter flex_row right_col flex_align_center gap_20 margin_t_nagative1 padding_l_48">
        <div v-for=" item in accountSImg">
          <img v-for="item in item.img" :src="item" alt="">
        </div>
      </div>
      
    </div>
  </div>
</template>
<style>
.account_page {
  background-image: linear-gradient(195deg,rgba(66, 66, 74, 0.5),rgba(25, 25, 25, 0.5)), url(https://demos.creative-tim.com/material-kit-pro/assets/img/shapes/pattern-lines.svg);
  background-color: #313135;
}
.right_col >* {
  width: 33.33%;
}
.right_col {
  
}
.account_page img {
  width: 100%;
  border-radius: 15px;
  margin-bottom: 15px;
  
}
</style>