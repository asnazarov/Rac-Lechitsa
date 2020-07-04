<template>
  <section id="rootSection" class="root-section">
    <div class="root-section__item">
      <h2 class="root-section__title">Истории людей, победивших рак, но не свои привычки</h2>
      <p class="root-section__text">Есть вещи, которые не лечатся. Вещи ставшие частью нашего «я», фобии, страхи. Но это точно не рак. Рак лечится. Лучшее доказательство — люди с их историями.</p>
      <nav-btn></nav-btn>
      <!-- <div class="nav-btn">
        <button class="nav-btn__left"></button>
        <button class="nav-btn__right"></button>
      </div> -->
    </div>
    <div class="root-section__video">
     <iframe class="root-section__video-item"  src="https://www.youtube.com/embed/Qb4KUktbpzQ" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      <figure>
      <figcaption class="root-section__figcaption">Все видео вы можете найте на нашем <a class="root-section__fig-link" target="_blank" href="https://www.youtube.com/channel/UCcxMSzN1R4JfW1vLu3swCaQ/featured">YouTube канале</a>.</figcaption>
      </figure>
    </div>


  </section>
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
.root-section {
  position: relative;
  max-width: 1440px;
  margin: 0 auto 0 auto;
  // padding-top: 100px;
  padding: 100px 60px 70px 60px;
  display: flex;
  justify-content: space-between;

		&__item {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
		}

		&__title {
      font-family: 'Inter',sans-serif;
      font-weight: 600;
      font-size: 32px;
      line-height: 36px;
      max-width: 330px;
      margin-bottom: 32px;
		}

		&__text {
      font-family: 'Inter',sans-serif;
      color: #666666;
      font-size: 18px;
      font-weight: normal;
      line-height: 22px;
      max-width: 340px;
      margin-bottom: auto;
		}

		&__video {
      max-width: 867px;
      max-height: 450px;
    }
    &__video-item{
      width: 867px;
      height: 450px;
      border-radius: 7px;
      border: none;
    }

		&__figcaption {
      font-family: 'Inter',sans-serif;
      margin-top: 10px;
      font-size: 12px;
      line-height: 16px;
      color: #666666;
    }
    &__fig-link {
      font-family: 'Inter',sans-serif;
      color: #666666;
    }
}

</style>
