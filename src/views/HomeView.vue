<template>
    <div>
    <TwoInOne :name="'Buy your favorite gifts around Europe with ' " :imgsrc="coll" :visit="'/about'" :btnName="'Get Started'"/>
    </div>
</template>

<script setup>
import TwoInOne from '../components/TwoInOne.vue'
import coll from '../assets/images/coll.jpg'
</script>

<style  scoped>

</style>