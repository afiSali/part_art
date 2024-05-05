<template>
    <div>
        <TwoInOne :name="'Welcome To About Page' " :imgsrc="coll" :visit="'/services'" :btnName="'Categories'"/>
    </div>
</template>

<script setup>
import TwoInOne from '../components/TwoInOne.vue'
import coll from '../assets/images/coll.jpg'
</script>

<style  scoped>

</style>