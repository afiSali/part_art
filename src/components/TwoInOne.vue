<template>
    <div class="container mx-auto px-5 lg:px-20 h-[100vh] md:h-[80vh] flex flex-col-reverse  md:flex-row  justify-center md:justify-center items-center gap-10">
       
            <div class="w-full flex  items-center flex-col md:items-start">
                <h1 class="text-2xl md:text-4xl text-slate-700 my-1">{{ name }} <br> <strong  class="text-blue-700 text-5xl lg:text-6xl font-bold">PartArt Team</strong></h1>
                <p class="text-2xl md:text-4xl text-slate-700 my-1"> We are the team of the talented artists</p>
                <router-link  :to="visit" class="bg-amber-400 hover:bg-blue-700 outline-none px-12 py-4 rounded-2xl mt-3 text-white text-xl font-medium">{{ btnName }}</router-link>
            </div>
            <div class="coll">
                <img :src="imgsrc" alt="team-img" class="w-[100%] h-[100%] mt-3">
            </div>
 
    </div>
</template>

<script setup>
import {defineProps} from 'vue'
import {RouterLink} from 'vue-router'
const props= defineProps(['name','imgsrc','visit','btnName'])
</script>

<style scoped>
.coll{
    animation: up-down 1s alternate infinite;
}
@keyframes up-down{
    0%{
        transform: translateY(10px);
    }
    100%{
        transform: translateY(-10px);
    }
}
</style>