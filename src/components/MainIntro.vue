<script setup>

</script>
<template>
  <div class="bg_pink position_relative">
    <div class="txt_center margin_auto width_mainintro flex_col flex_justify_center position_absolute">
      <h1 class="txt_white fontsz_7">Material Kit 2 PRO</h1>
      <p class="txt_white fontsz_3 line_height_4 width_p margin_y_15">Start the Development With A Bootstrap 5 Design System inspired by Material Design.</p>
    </div>
  </div>
</template>
<style>

.bg_pink{
  background-image: -webkit-linear-gradient(90deg,rgba(236, 65, 122, 0.45) 0,rgba(216, 27, 96,0.65) 180%), url('https://demos.creative-tim.com/material-kit-pro/assets/img/bg0.jpg');
  background-position: center center;
  background-size: cover;
  background-repeat: no-repeat;
  min-height: 75vh;
}
.position_relative {
  position: relative;
}
.position_absolute {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.width_p {
  width: 550px;
}
</style>
