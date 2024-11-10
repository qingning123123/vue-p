<template>
    <button :class="{but1: disabled , but2: !disabled ,but3: size === 'small', but: size !== 'small'}">
    {{ text }}
  </button>
</template>

<script setup>
defineProps({
  text: String,
  disabled: Boolean,
  size: String,
})

</script>

<style scoped>
.but {
  width: 166px;
  height: 44px;
  border-radius: 4px;
  font-size: 16px;
  line-height: 16px;
}

.but1 {
  background: #E7E8EA;
  color: rgba(125, 145, 157, 0.50);
}

.but2 {
  margin-left: 10px;
  margin-right: 10px;
  background: #0062F8;
  color: #FFF;
}

.but3 {
  width: 72px;
  height: 28px;
  border-radius: 6px;
  background: #0062F8;
  color: #FFF;
  font-size: 12px;
  line-height: 12px;
}

</style>