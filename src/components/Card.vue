<template>
    <div class="bg-white shadow-lg rounded-lg">
      <img  :src="imgsrc" :alt="title" class="w-full object-cover h-[200px] rounded-t-lg hover:scale-90 duration-300">
    
    <div class="text p-9 font-bold tex-lg">
        <h2 class="text-slate-950 py-1">{{ title }}</h2>
        <h2 class="text-slate-800 py-1 font-medium text-base">Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit, nesciunt?</h2>
        <button class="bg-blue-600 hover:bg-amber-300 outline-none px-10 py-3 rounded-2xl mt-3 text-white text-xl font-medium">Shopping</button>

    </div>
  </div>
</template>


<script setup>
import {defineProps} from 'vue'
const props= defineProps(['imgsrc','title'])
</script>

<style  scoped>

</style>