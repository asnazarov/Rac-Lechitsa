<template>
  <div class="nav-btns-wrapper">
    <button class="nav-btn nav-btn_left"></button>
    <button class="nav-btn nav-btn_right"></button>
  </div>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>
.nav-btns-wrapper {
  display: flex;
}
.nav-btn {
padding: 0;
margin: 0;
background-color: #613A93;
border: none;
width: 40px;
height: 40px;
background-repeat: no-repeat;
background-position: center;

		&_left {
      background-image: url(../../static/images/ui/left-gray.svg);
      border-top-left-radius: 4px;
      border-bottom-left-radius: 4px;
		}

		&_right {
      background-image: url(../../static/images/ui/right-gray.svg);
      border-top-right-radius: 4px;
      border-bottom-right-radius: 4px;
		}
}
.nav-btn_left:focus {
  content: '';
  background-image: url(../../static/images/ui/left-white.svg);
  outline: none;
}
.nav-btn_right:focus {
  background-image: url(../../static/images/ui/right-white.svg);
  outline: none;
}
.nav-btn_left:hover, .nav-btn_right:hover {
  opacity: 0.9;
}
</style>
