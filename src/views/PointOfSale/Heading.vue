<template>
    <div class="flex justify-between sm:mx-6 sm:py-3">
      <h1 class="text-2xl">Punto de venta</h1>
      <button @click="toggleDarkMode" class="bg-white dark:bg-[#363B3D]  border text-xl p-2 rounded-2xl dark:border-0">
        Mode Switch
      </button>
    </div>
  </template>
  
  <script>
  export default {
    name: "Heading",
    data() {
      return {
        isDarkMode: false,
      };
    },
    methods: {
      toggleDarkMode() {
        this.isDarkMode = !this.isDarkMode;
        document.documentElement.classList.toggle('dark', this.isDarkMode); 
      },
    },
  };
  </script>



  
 
  
