<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <MyContentIcon/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyFooter from './components/MyFooter.vue'
import MyContentIcon from './components/MyContentIcon.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter,
    MyContentIcon
}
}
</script>

<style lang="scss">

  

</style>
