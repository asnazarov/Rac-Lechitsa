<template>
  <div class="popup">
    <slot>
      <p class="popup__counter">Шаг 1 из 12</p>
      <p class="popup__text">Как вас зовут?</p>
      <input class="popup__input" type="text" placeholder="Напишите тут">
      <!-- <nav-btn @click="$emit('btnNextPopup')"></nav-btn> -->
      <img class="popup__close" @click="$emit('popupClose')" src="../static/images/ui/popup-close.png" alt="">
    </slot>
      <button @click="$emit('btnNextPopup')">Дальше</button>
  </div>
</template>

<script>
import NavBtn from '@/components/ui/NavBtn'
  export default {
    components: {
      'nav-btn': NavBtn,
    },
  }
</script>

<style lang="scss" scoped>
.popup {
  background-color: white;
  width: 920px;
  height: 600px;
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  flex-direction: column;
  z-index: 11;
  padding: 40px;
  font-family: 'Inter', sans-serif;
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
		&__counter {
      font-weight: 600;
      font-size: 32px;
      line-height: 36px;
		}

		&__text {
      font-weight: 500;
      font-size: 18px;
      line-height: 24px;
      margin-top: 40px;
		}

		&__input {
      width: 100%;
      height: 40px;
      margin: auto 0;
      border: 0;
      border-bottom: 1px solid #b1b1b1;
      font-weight: normal;
      font-size: 18px;
      line-height: 24px;
    }
    &__close {
      position: absolute;
      top: 35px;
      right: 35px;
    }
}
.popup__input:focus{
  border: 0;
  border-bottom: 1px solid #0c0c0c;
  outline: none;
}
.popup__close:hover{
  cursor: pointer;
}
</style>
