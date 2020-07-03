<template>
  <nav class="navigation">
    <ul class="menu">
      <li><nuxt-link class="menu__link" to="/">Главная</nuxt-link></li>
      <li><nuxt-link class="menu__link" to="/stories">Истории</nuxt-link></li>
      <li><nuxt-link class="menu__link menu__link_anotherColor" to="/">Рассказать историю</nuxt-link></li>
    </ul>
  </nav>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>
.navigation {
margin: auto 60px auto auto;
}
.menu {
  box-sizing: border-box;
display: flex;
flex-wrap: wrap;
justify-content: space-between;
list-style-type: none;
padding: 0;
margin-left: -40px;

		&__link {
      margin-left: 40px;
      font-family: 'Inter', sans-serif;
      font-weight: normal;
      font-size: 18px;
      line-height: 24px;
      color: #000;
      text-decoration: none;
      &_anotherColor {
        background-color: #613A93;
        padding: 12px 20px;
        color: #fff;
      }
      &_active {
        border-bottom: 1px solid #000;
      }
		}
}

</style>
