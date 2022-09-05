<template>
  <div class="debug" id="app">
    <MyTopbar />
    <MyMain />
    <MyFooter />
  </div>
</template>

<script>
import MyTopbar from '@/components/MyTopbar.vue'
import MyMain from '@/components/MyMain.vue'
import MyFooter from '@/components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MyTopbar,
    MyMain,
    MyFooter
  }
}
</script>

<style lang="scss">
@import '@/styles/vars.scss';
@import '@/styles/debug.scss';
@import '~@fortawesome/fontawesome-free/css/all.css';

@import '@/styles/general.scss';
@import '@/styles/common.scss';

</style>
