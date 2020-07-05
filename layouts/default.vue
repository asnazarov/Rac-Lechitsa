<template>
  <div>
    <myHeader @clickHistory="popupHandler"></myHeader>
    <Nuxt />
    <overlay v-if="PopupShow" @clickOverlay="popupHandler"></overlay>
    <popup class="popup" v-if="PopupShow" @popupClose="popupHandler" @btnNextPopup="nextPopup">
    </popup>
    <popup v-if="PopupShow1">
      <p class="popup__counter">Шаг 2 из 12</p>
      <p class="popup__text">Было ли у вас онкологическое заболевание? Если да – расскажите, пожалуйста, кратко, какой диагноз и текущий статус. Если нет — приглашаем Вас поделиться своей историей неизлечимых привычек в Инстаграм с хештегами #раклечится и #этонелечится.</p>
      <input class="popup__input" type="text" placeholder="Напишите тут">
    </popup>
    <popup v-if="PopupShow1">
      <p class="popup__counter">Шаг 3 из 12</p>
      <p class="popup__text">Было ли у вас онкологическое заболевание? Если да – расскажите, пожалуйста, кратко, какой диагноз и текущий статус. Если нет — приглашаем Вас поделиться своей историей неизлечимых привычек в Инстаграм с хештегами #раклечится и #этонелечится.</p>
      <input class="popup__input" type="text" placeholder="Напишите тут">
    </popup>
  </div>
</template>

<script>
import Header from '@/components/Header';
import Overlay from '@/components/ui/Overlay';
import Popup from '@/components/Popup';
export default {

  data() {
    return {
      PopupShow: false,
      PopupShow1: false,
    };
  },
   components: {
    'myHeader': Header,
    'overlay': Overlay,
    'popup': Popup,
  },
   methods: {
     nextPopup () {
       const a = this.$el.querySelector(".popup")
      // console.log(a == false)
      if (a!=true){
        this.PopupShow = !this.PopupShow
        this.PopupShow1 = !this.PopupShow1
      } else {
        console.log('4444444444')
      }
    },
    popupHandler () {
      this.PopupShow = !this.PopupShow


    },

  },
}
</script>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
