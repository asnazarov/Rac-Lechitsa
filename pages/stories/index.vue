<template>
  <div class="container">
    <logo></logo>
    all stories
  </div>
</template>

<script>
import Logo from '@/components/Logo';
export default {
  components: {
    Logo: Logo,
  },
};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
