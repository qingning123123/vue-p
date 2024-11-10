<script setup>
import ViButton from './components/ViButton.vue'
</script>

<template>
  <div>
    <!-- <button class="but but1">59s后自动取消</button>
    <button class="but but2">下单</button>
    <button class="but3">上传</button> -->

    <ViButton :disabled="true" text="59s后自动取消"></ViButton>
    <ViButton text="下单"></ViButton>
    <ViButton size="small" text="上传"></ViButton>
  </div>
</template>
