<script setup lang="ts">
import Details from '@/views/CheckoutPage/Details.vue';
import Options from '@/views/CheckoutPage/Options.vue';
import PriceSection from '@/views/CheckoutPage/PriceSection.vue';
import TableSection from '@/views/CheckoutPage/TableSection.vue';

</script>

<template>
  <Options/>
  <!-- <div class="inline-block">
    <Details/>
    <TableSection/>  
  </div>
  <div class="inline-flex h-100">
      <PriceSection/>
  </div> -->
  <div class="flex">
    <div >
      <Details/>
    <TableSection/>
    </div>
    <div class="">
      <PriceSection/>
    </div>
  </div>


</template>

