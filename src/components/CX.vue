<script setup>
import CardBorder from './CardBorder.vue';

</script>
<template>
  <div class="max_width_card margin_auto">
    <div class="flex_row gap_20">
      <CardBorder
        :bgColor="'four'"
        :useShadow="false"
        :icon="'bi bi-clock txt_lightgray'"
        :position="'bottom'"
        :txtCol="'txt_lightgray'"
        :txtColor1="'txt_darkgray'"
        :txtColor2="'txt_lightgray'"
        :txtColor3="'txt_lightgray'"
      >
        <template #note>  1 day ago</template>
        <template #title>Nick Willever</template>
        <template #decription>"This is an excellent product, the documentation is excellent and helped me get things done more efficiently."</template>
        
        <template #last><i class="bi bi-star-fill"></i>  <i class="bi bi-star-fill"></i>  <i class="bi bi-star-fill"></i>  <i class="bi bi-star-fill"></i>  <i class="bi bi-star-fill"></i></template>
      </CardBorder>
      <CardBorder
        :bgColor="'main'"
        :useShadow="true"
        :icon="'bi bi-clock txt_white'"
        :position="'bottom'"
        :txtCol="'txt_white'"
        :txtColor1="'txt_white'"
        :txtColor2="'txt_white'"
        :txtColor3="'txt_white'"
      >
        <template #note> 1 week ago</template>
        <template #title>Shailesh Kushwaha</template>
        <template #decription>"I found solution to all my design needs from Creative Tim. I use them as a freelancer in my hobby projects for fun! And its really affordable, very humble guys !!!"</template>
        <template #last><i class="bi bi-star-fill"></i>  <i class="bi bi-star-fill"></i>  <i class="bi bi-star-fill"></i>  <i class="bi bi-star-fill"></i>  <i class="bi bi-star-fill"></i></template>
      </CardBorder>
      <CardBorder
        :bgColor="'four'"
        :useShadow="false"
        :icon="'bi bi-clock txt_lightgray'"
        :position="'bottom'"
        :txtCol="'txt_lightgray'"
        :txtColor1="'txt_darkgray'"
        :txtColor2="'txt_lightgray'"
        :txtColor3="'txt_lightgray'"
      >
        <template #note> 3 weeks ago</template>
        <template #title>Samuel Kamuli</template>
        <template #decription>"Great product. Helped me cut the time to set up a site. I used the components within instead of starting from scratch. I highly recommend for developers who want to spend more time on the backend!."</template>
        <template #last><i class="bi bi-star-fill"></i>  <i class="bi bi-star-fill"></i>  <i class="bi bi-star-fill"></i>  <i class="bi bi-star-fill"></i>  <i class="bi bi-star-fill"></i></template>
      </CardBorder>
      
    </div>

  </div>
</template>