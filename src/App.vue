<script setup>
import ViButton from './components/ViButton.vue'
import Datapresent from './components/Datapresent.vue';
</script>

<template>
  <div>
    <!-- <button class="but but1">59s后自动取消</button>
    <button class="but but2">下单</button>
    <button class="but3">上传</button> -->

    <ViButton :disabled="true" text="59s后自动取消"></ViButton>
    <ViButton text="下单"></ViButton>
    <ViButton text="89293233232" text2="dcawsdaawd"></ViButton>
    <ViButton size="small" text="上传"></ViButton>
  </div>
  <div>
    <Datapresent length="all" background="red" :color="true" leftText="68881.9693" rightText="0.0002890"></Datapresent>
    <Datapresent background="red" :color="true" leftText="68881.9693" rightText="0.0002890"></Datapresent>
    <Datapresent length="all" background="red" leftText="68881.9693" rightText="0.0002890"></Datapresent>
    <Datapresent background="red" leftText="68881.9693" rightText="0.0002890"></Datapresent>
  </div>

</template>
