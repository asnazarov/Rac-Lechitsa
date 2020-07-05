<template>
  <header class="header">
    <h1 class="header__title">Проект Благотворительного Фонда Константина Хабенского</h1>
    <myMe @clickHistory="$emit('clickHistory')"></myMe>
  </header>
</template>

<script>
import Menu from '@/components/Menu'
  export default {
   components: {
    'myMe' : Menu,
  },
  }
</script>

<style lang="scss" scoped>
.header {
max-width: 1440px;
margin: 0 auto;
min-height: 76px;
border: 1px solid green;
display: flex;
justify-content: space-between;
		&__title {
      box-sizing: border-box;
      margin: auto 40px auto 60px;
      max-width: 340px;
      min-width: 300px;
      border: 1px solid rgb(128, 0, 0);
      font-family: 'Inter', sans-serif;
      font-weight: 600;
      font-size: 16px;
      line-height: 20px;
		}
}


</style>
