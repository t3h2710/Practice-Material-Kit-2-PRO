<script setup>
import Button from './Button.vue';
</script>
<template>
  <div class="account_page flex_justify_center flex">
    <div class="flex_row max_width_card ">
      <div class="width_quarter left_col flex_col flex_justify_center">
        <h2 class="txt_white fontsz_4 font_weight_7 line_height_2 margin_b_20">Account Pages for beautiful webapps</h2>
        <span class="line_height_2 margin_b_20 fontsz_1 font_weight_1 txt_p">We created many examples for pages like Signup, Signin, Forgot Password, 2FA Authentification and so on. Just choose between a Basic Design, an illustration or a cover and you are good to go!</span>
        <div>
          <Button>VIEW PAGES</Button>
          <Button
            :bg-color="'bg_transparent'"
          >
            VIEW SIGNUP PAGES
          </Button>
        </div>
        
      </div>
      <div class="width_three_quarter flex_row right_col flex_align_center gap_20 margin_t_nagative1 padding_l_48">
        <div class="">
          <img src="https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/account/sign-up-cover.jpg" alt="">
          <img src="https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/account/reset-cover.jpg" alt="">
          <img src="https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/account/signup-illustration.jpg" alt="">
        </div>
        <div class="">
          <img src="https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/account/2fa.jpg" alt="">
          <img src="https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/account/comming-soon.jpg" alt="">
          <img src="https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/account/reset-basic.jpg" alt="">
          <img src="https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/account/error-500.jpg" alt="">
        </div>
        <div class="">
          <img src="https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/account/error-404.jpg" alt="">
          <img src="https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/account/signin-basic.jpg" alt="">
          <img src="https://raw.githubusercontent.com/creativetimofficial/public-assets/master/material-design-system/presentation/account/sign-up-cover.jpg" alt="">

        </div>
      </div>
      
    </div>
  </div>
</template>
<style>
.account_page {
  background-image: url(https://demos.creative-tim.com/material-kit-pro/assets/img/shapes/pattern-lines.svg), linear-gradient(195deg,#42424a,#191919);
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