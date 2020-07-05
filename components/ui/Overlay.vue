<template>
  <div class="overlay" @click="$emit('clickOverlay')">
    <!-- <popup @popupClose="$emit('popupClose')"></popup> -->
  </div>
</template>

<script>
import Popup from '@/components/Popup'
  export default {
    components: {
      'popup': Popup
    }
  }
</script>

<style lang="scss" scoped>
.overlay {
  // display: block;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  position: fixed;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  background: rgba(0, 0, 0, 0.5);
  z-index: 10;
}
</style>
