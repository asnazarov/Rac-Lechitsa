<template>
  <div class="callout">
    <slot><h2 class="callout__title">И В ОТЛИЧИЕ ОТ РАКА, <span class="callout__hashtag">#ЭТОНЕЛЕЧИТСЯ</span></h2></slot>
  </div>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>
.callout {
width: 1440px;
background-color: #613A93;
min-height: 86px;
margin: 0 auto 20px auto;
display: flex;
justify-content: center;
align-items: center;
flex-direction: column;

		&__title {
      font-family: 'Inter', sans-serif;
      letter-spacing: 2px;
      text-align: center;
      max-width: 700px;
      color: white;
      font-size: 20px;
      line-height: 46px;
      font-weight: 400;
		}

		&__hashtag {
      letter-spacing: 0px;
      font-size: 30px;
      line-height: 46px;
      font-weight: 700;
		}
}

</style>
