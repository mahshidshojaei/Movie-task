<script setup>
import MovieCard from '../components/MovieCard.vue';
import Player from '../components/Player.vue'

</script>
<template>
  <div class="flex flex-col">
    <div class="text-end">
      <button
        class="bg-[#242629] rounded-[4px] text-[15px] px-[18px] py-[12px]"
      >
        <span>بازگشت</span>
        <i class="ki-filled ki-left text-[10px] mr-[2px] p-1"></i>
      </button>
    </div>
    <div class="grid grid-cols-2 items-center mt-[4px]">
      <div class="flex items-center gap-[8px]">
        <div
          class="bg-[#AB070F] rounded-[4px] p-[2px] flex flex-col items-center gap-[6px] w-[42px] h-[43px]"
        >
          <div
            class="bg-[#F2F2F2] text-[13px] rounded-[3px] p-[2px] text-[#AB070F] text-center font-black w-[38px] h-[19px]"
          >
            1080
          </div>
          <span class="text-[#FFFFFF] text-[10px] font-bold">WebDL</span>
        </div>
        <div class="flex flex-col">
          <span class="text-[25px] font-black">فیلم EL CAMINO</span>
          <span class="text-[14px] font-normal">فیلم ال کامینو</span>
        </div>
      </div>
      <div class="grid grid-cols-6 items-center">
        <div
          class="col-span-2 bg-[#242629] rounded-[4px] flex gap-[10px] items-center justify-center text-[15px]  h-[48px]"
        >
          <span> کیفیت 1080p - webdl</span>
          <i class="ki-filled ki-down text-[#9DA5B2] w-[20px] h-[20px]"></i>
        </div>

        <div class="col-span-2 flex gap-[7px] text-yellow-400 text-3xl text-[23px] justify-center">
          <i class="fa-solid fa-star text-[#5A5E66]"></i>
          <i class="fa-solid fa-star text-[#5A5E66]"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
          <i class="fa-solid fa-star"></i>
        </div>
        <div class="col-span-1 flex items-center gap-1 justify-end">
        <div class="font-black text-[20px]">
              <span class="">۱۰</span>
              /
              <span class="text-[24px]">۴.۵</span>
        </div>
        <img src="../assets/images/IMDB.png" alt="">
       </div>
        <div class="col-span-1 flex gap-[8px] justify-end">
              <div
                  class="bg-[#242629] w-[45px] h-[45px] rounded-[4px] flex items-center justify-center"
                >
                <i class="fa-regular fa-share-nodes"></i>
                </div>
                <div
                  class="bg-[#242629] w-[45px] h-[45px] rounded-[4px] flex items-center justify-center"
                >
                <i class="fa-light fa-bookmark"></i>
                </div>
        </div>
      </div>
    </div>
    <div class="grid grid-cols-3 mt-[8px]">
       <div class="col-span-2">
        <Player />
        <div class="flex w-full justify-between mt-4">
        <div class="flex gap-1">
          <span class="bg-[#AB070F99] rounded-[4px] p-[12px] text-[13px] font-black">پلیر تلوزیون های سامسونگ</span>
          <span class="bg-[#242629] rounded-[4px] p-[12px] text-[13px] font-black">پلیر تلوزیون های قدیمی</span>
          <span class="bg-[#242629] rounded-[4px] p-[12px] text-[13px] font-black">پلیر تلوزیون های قدیمی</span>
        </div>
        <div class="flex items-center gap-[4px]">
          <span class="text-[#9DA5B2] text-[12px]">حین تماشا با مشکلی رو به رو شدید؟</span>
          <span class="underline decoration-1 bg-[#242629] p-[8px] rounded-[4px] text-[12px]">اعلام مشکل</span>
        </div>
      </div>
       </div>
       <div class="col-span-1 flex flex-col items-center gap-2">
              <MovieCard/>
              <MovieCard/>
              <MovieCard/>
        <span class="text-[14px] flex gap-2 items-center mt-[16px]">مشاهده همه فیلم ها<i class="fa-regular fa-arrow-left"></i></span>
       </div>
    </div>
  </div>
</template>
