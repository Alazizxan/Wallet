<script setup>
import {defineProps} from 'vue'

defineProps({
  friendName: String,
  money: String,
  date: String,
  clock: String
})
</script>

<template>
<div class="friend task w-[91%] m-auto rounded-[12px] h-[67px] px-[16px] py-[10px] flex items-center justify-between  bg-bgGray">
  <div class="profile flex items-center gap-[10px]">
    <img class="w-[36px]" src="../assets/images/profile.svg" alt="profile">

    <div class="profile__text flex flex-col">
      <span class="text-[17px] text-white font-main">{{friendName}}</span>
      <span class="text-[12px] text-mainGray font-ibm">{{money}} BW</span>
    </div>
  </div>

  <div class="date flex flex-col">
    <span class="font-ibm text-mainGray text-[10px]">{{date}}</span>
    <span class="font-ibm text-mainGray text-[10px]">{{clock}}</span>
  </div>
</div>
</template>

<style scoped>

</style>