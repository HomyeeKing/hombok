<script setup lang="ts">
import Card from '@/components/Card.vue'
import Categories from '@/category'
</script>

<template>
    <h1 class="text-blue-800 underline text-2xl italic">HOMBOK!</h1>
    <small class="capitalize ml-70">—— the intelligence of homyee king</small>
    <div v-for="{name,createTime} in Categories" :key="createTime">
        <Card :name='name' :create-time="createTime" />
    </div>
</template>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
