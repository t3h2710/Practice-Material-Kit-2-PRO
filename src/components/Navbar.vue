<script setup>
  import CardWhite from './CardWhite.vue'
  import NavbarLink from './NavbarLink.vue';
  import Button from './Button.vue';

</script>

<template>
  <div class="navbar padding_y_16 ">
    <CardWhite class="flex flex_space_between flex_align_center padding_x_15 padding_y_10 max_width_card margin_auto">
      <div>
        <span class="txt_darkgray margin_l_15 font_weight_5">Material Kit 2 PRO</span>
      </div>
      <div class="flex_row gap_10">
        <NavbarLink 
          :imgLeft="'/img/icon_layout.png'" 
          :imgRight="'https://demos.creative-tim.com/material-kit-pro/assets/img/down-arrow-dark.svg'"
        >
          Pages
        </NavbarLink>
        <NavbarLink 
          :imgLeft="'/img/icon_layout.png'" 
          :imgRight="'https://demos.creative-tim.com/material-kit-pro/assets/img/down-arrow-dark.svg'"
        >
          Account
        </NavbarLink>
        <NavbarLink 
          :imgLeft="'/img/icon_layout.png'" 
          :imgRight="'https://demos.creative-tim.com/material-kit-pro/assets/img/down-arrow-dark.svg'"
        >
          Sections
        </NavbarLink>
        <NavbarLink 
          :imgLeft="'/img/icon_layout.png'" 
          :imgRight="'https://demos.creative-tim.com/material-kit-pro/assets/img/down-arrow-dark.svg'"
        >
          Docs
        </NavbarLink>
        <Button>BUY NOW</Button>        
      </div>
    </CardWhite>
    
  </div>
</template>

<style>
.navbar {
  position: fixed;
  top: 0;
  
  z-index: 100;
  width: 100%;
}

.navbar .icon {
  width: 20px;
}

.navbar a {
  margin: 0 10px;
}

</style>