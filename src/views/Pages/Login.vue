<script setup lang="ts">
import Show from "@/assets/vueJs/view.png";
import Hide from "@/assets/vueJs/hide.png";

let a: boolean = false;

function pass() {
  const passwordInput = document.getElementById("password");
  const passIcon = document.getElementById("pass-icon");

  if (passwordInput && passIcon) {
    if (a) {
      passwordInput.type = "password";
      passIcon.src = Hide;
      a = false;
    } else {
      passwordInput.type = "text";
      passIcon.src = Show;
      a = true;
    }
  }
}
</script>

<template>
  <div
    class="bg-[url('@/assets/vueJs/Background.png')] bg-cover h-screen bg-no-repeat text-white"
  >
    <div class="w-fit mx-auto pt-46">
      <img class="w-70 sm:w-90" src="@/assets/vueJs/Logo.png" alt="" />
    </div>
    <div
      class="border-2 border-[black] bg-white text-black mt-16 w-[60%] sm:w-[235px] mx-auto rounded-[40px]"
    >
      <div>
        <p class="font-light text-[#62666F] text-4xl text-center py-[25px]">
          Bienvenido
        </p>
        <input
          class="border-b border-[#aaaeb6] ml-[23px] pl-[5px] outline-none text-[20px] w-[80%] mb-[15px] sm:mb-[30px]"
          type="text"
          placeholder="usuario"
        />
        <input
          class="border-b border-[#aaaeb6] ml-[23px] pl-[5px] outline-none text-[20px] w-[80%]"
          type="password"
          id="password"
          placeholder="contrasena"
        />
        <img
          src="@/assets/vueJs/hide.png"
          @click="pass"
          class="relative ml-[80%] -mt-5 cursor-pointer"
          id="pass-icon"
        />
        <div class="flex ml-[23px] pt-2 pb-5 gap-1">
          <input class="" type="checkbox" />
          <p class="text-body text-[12px]">Recuerdame</p>
        </div>
      </div>
      <div class="w-fit mx-auto sm:mb-[-20px] mb-[-9%]">
        <button
          class="text-[#b3b8c4] font-extralight bg-[#525659] py-2 px-3 sm:px-6 rounded-full text-2xl"
        >
          lniciar sesion
        </button>
      </div>
    </div>
  </div>
</template>
