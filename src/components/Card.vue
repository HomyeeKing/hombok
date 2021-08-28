<script lang='ts' setup>
import { defineProps } from 'vue'
import type { Card } from '@/types'

defineProps<Card>()
</script>

<template>
    <div class="w-2/5 h-32 border border-solid flex justify-center items-center flex-col">
       <span class="text-4xl">{{name}}</span>
       <span>{{`创建时间： ${createTime}`}}</span>
    </div>
</template>
