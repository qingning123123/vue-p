<template>
    <div :class="{por: true,height: true,flex: true, tap_text: true}">
    <div :class="{
      poa: true,height: true, tap_bgct: background, tap_bgcf: !background,
      tap_all: length === 'all', tap_short:length !== 'all'}"> </div>
    <p :class="{tap_leftt: background , tap_leftf: !background}">{{ lefttext }}</p>
    <p :class="{tap_right: true}">{{ righttext }}</p>
    </div>
</template>

<script setup>
defineProps({
  length: String,
  background: Boolean,
  lefttext: String,
  righttext: String,
})

</script>

<style scoped>


.flex {
  display: flex;
  justify-content:space-between;
  align-items:center;
}

.por{
  position:relative;
}
.height {
  height: 22px;
}

.poa {
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
}

.tap_text {
  width: 149px;
  font-size: 12px;
  font-weight: 700;
  line-height: 12px;

}

.tap_leftt {
  color: #DF294A;
}

.tap_right {
  color:  #333;
}

.tap_leftf {
  color: #00AF8E;
}


.tap_bgct {
  background: #FCE9EB;


}
.tap_bgcf {
  background: #E9F8F3;
}

.tap_all {
  width: 149px;
}

.tap_short {
  width: 10px;

}


</style>