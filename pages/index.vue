<template>
  <div class="container">
    <myCover ></myCover>
    <rootSection ></rootSection>
    <callout></callout>
    <callout>
      <h2 class="callout__title">РАССКАЗЫВАЙТЕ ВАШИ ИСТОРИИ В ИНСТАГРАМ <span class="callout__hashtag">#ЭТОНЕЛЕЧИТСЯ #РАКЛЕЧИТСЯ</span></h2>
    </callout>
    <logo></logo>
    <h1 class="title">Hello</h1>
    <input type="text" name v-model="text" />
    <p class="subtitle">{{ text }}</p>
    <a href="http://localhost:3000/stories">About</a>
  </div>
</template>

<script>
import Cover from '@/components/Cover'
import RootSection from '@/components/RootSection'
import Callout from '@/components/Callout'

import Logo from '@/components/Logo';
export default {
  data() {
    return {
      PopupShow: false,
      text: 'YoYoYo',
    };
  },
  components: {
    logo: Logo,
    myCover: Cover,
    'rootSection': RootSection,
    'callout': Callout,
  },
};
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
}

.title {
  /* font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif; */
    /* font-family: "Inter", "Source Sans Pro"; */
    font-family: "Inter", sans-serif;
  display: block;
  font-weight: 500;
  /* font-weight: 300; */
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
