<template>
  <section id="rootSection" class="root-section">
    <div class="root-section__item">
      <h2 class="root-section__title">Истории людей, победивших рак, но не свои привычки</h2>
      <p class="root-section__text">Есть вещи, которые не лечатся. Вещи ставшие частью нашего «я», фобии, страхи. Но это точно не рак. Рак лечится. Лучшее доказательство — люди с их историями.</p>
      <nav-btn></nav-btn>
    </div>
    <div class="root-section__video">
     <iframe class="root-section__video-item"  src="https://www.youtube.com/embed/Qb4KUktbpzQ"
     allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
     allowfullscreen seamless></iframe>
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
      width: 40%;
      margin-right: 15px;
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
      width: 60%;
      padding-bottom: calc(9 * 60% / 16);
      position: relative;
      align-self: flex-start;
    }

    &__video-item{
      width: 100%;
      height: 93%;
      position: absolute;
      top: 0;
      left: 0;
      border-radius: 7px;
      border: none;

    }

		&__figcaption {
      position: absolute;
      left: 0;
      bottom: 0;
      font-family: 'Inter',sans-serif;
      margin-top: 20px;
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
