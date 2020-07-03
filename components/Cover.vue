<template>
  <section class="cover">
    <h2 class="cover__title">#РАКЛЕЧИТСЯ</h2>
    <nuxt-link class="cover__link" to="/"><img src="../static/images/cover/cover__link.png" alt=""></nuxt-link>
  </section>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>
.cover {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  min-height: 90vh;
  background-color: #613A93;

		&__title {
      color: #fff;
      font-family: 'Inter', sans-serif;
      font-weight: 800;
      font-size: 92px;
      line-height: 111px;
		}

		&__link {
      position: absolute;
      bottom: 40px;
      right: 0 auto;
    }
}
</style>
