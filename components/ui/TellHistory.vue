<template>
  <button :class="['tellHistory', `tellHistory_theme_${theme}`]" @click="$emit('clickHistory')">
    <slot></slot>
  </button>
</template>

<script>
  export default {
    props: ['theme'],
  }
</script>

<style lang="scss" scoped>
.tellHistory{
  border: none;
  box-sizing: border-box;
  border-radius: 4px;
  color: #fff;
  &_theme_dark {
    background-color: #613A93;
    padding: 12px 20px;
    color: #fff;
    border: 4px solid transparent;
  }
  &_theme_light {
    background-color: #fff;
    padding: 12px 20px;
    color: #000;
    border: 4px solid #613A93;
  }
}
.tellHistory:hover {
  opacity: 0.9;
  cursor: pointer;
}
.tellHistory:focus {
  outline: none;
}
</style>
