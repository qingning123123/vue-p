<template>
  <div :class="{por: true , height: true , flex: true, tap_text: true}">
    <div
      :class="{poa: true , height: true , tap_all: length === 'all', tap_short: length !== 'all'}"
      :style="{background: background}"
      >
    </div>
    <p :class="{tap_leftt: color , tap_leftf: !color}">{{ leftText }}</p>
    <p :class="{tap_right: true}">{{ rightText }}</p>
  </div>
</template>

<script setup>
defineProps({
  length: String, //背景色长度
  color: Boolean, //文字颜色
  leftText: String,  //左边文字
  rightText: String,  //右边文字
  background:String,  //背景色颜色
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
  right: 0;
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

.tap_all {
  width: 149px;
}

.tap_short {
  width: 10px;
}
</style>