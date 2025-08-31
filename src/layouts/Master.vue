<script setup>
const menuIcons = ["notification", "save-2", "magnifier", "profile-circle"];
</script>

<template>
  <div class="layout flex flex-col h-screen bg-[#1B1C1F]">
    <div class="bg-[#242629]">
      <div class="container flex flex-col flex-1 justify-center">
        <div class="flex items-center justify-between">
          <div class="flex items-center gap-[24px] p-[12px]">
            <a href="#"
              ><img src="../assets/images/logo.png" class="h-10" alt="Logo"
            /></a>
            <div
              class="flex gap-[24px] text-[14px] leading-[20px] font-normal"
              dir="rtl"
            >
              <router-link to="/category" class="text-white"
                >دسته بندی ها</router-link
              >
              <router-link to="/film" class="text-white">فیلم</router-link>
              <router-link to="/series" class="text-white">سریال</router-link>
              <router-link to="/actors" class="text-white"
                >بازیگران</router-link
              >
              <router-link to="/newest" class="text-white"
                >جدید ترین دوبله ها</router-link
              >
            </div>
          </div>
          <div class="flex gap-[4px] items-center">
            <i class="ki-filled ki-left text-[#5A5E66] text-[12px]"></i>
            <div class="flex gap-[4px] py-[8px]">
              <div v-for="(icon, index) in menuIcons" :key="index">
                <div
                  class="bg-[#1B1C1F] w-[48px] h-[48px] rounded-[4px] flex items-center justify-center"
                >
                  <i
                    :class="`ki-outline text-[20px] text-white ki-${icon}`"
                  ></i>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <main class="flex-1 py-6 text-white container">
      <router-view />
    </main>
  </div>
</template>

<style scoped></style>
