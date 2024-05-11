<script setup lang="ts">

</script>
<template>
  <div class="bg-white shadow-4 p-3 rounded-xl relative h-full ">
    <div class="flex items-center justify-between mb-4">
      <p class="font-extrabold ">SubTotal</p>
      <p class="text-4xl font-thin">$3547.00</p>
    </div>
    <div class="flex items-center justify-between mb-4">
      <p class="font-extrabold  ">Descuento</p>
      <p class="text-4xl font-thin">$347.00</p>
    </div>
    <div class="flex items-center justify-between mb-4">
      <p class="font-extrabold ">Total</p>
      <p class="text-4xl text-black-2 font-bold">$3547.00</p>
    </div>
    <div class="flex justify-between gap-5">
      <button class=" bg-[#E6E6E7] px-3 py-3  text-black text-xl leading-none  rounded-md focus:outline-none">
        Efectivo
      </button>
      <button class=" bg-[#E6E6E7] px-2 py-3  text-black text-xl leading-none  rounded-md focus:outline-none">
        Tarjeta <br>Debito
      </button>
      <button class=" bg-[#E6E6E7] px-2 py-3   text-black text-xl leading-none  rounded-md focus:outline-none">
        tarjita <br> Credito
      </button>
    </div>
    <div class="flex justify-center my-4 absolute -bottom-10 left-20" >
      <button class=" bg-[#62666f] px-7 pt-2 pb-3 text-center mx-auto text-white text-3xl font-thin  rounded-full focus:outline-none">
      procesar
    </button>
    </div>
  </div>
</template>
