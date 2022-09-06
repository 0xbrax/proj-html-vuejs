<template>
  <div id="app">
    <MyHeader :checkScroll="isWindowScroll" />
    <MyMain />
    <MyFooter />
  </div>
</template>

<script>
import MyHeader from '@/components/MyHeader.vue'
import MyMain from '@/components/MyMain.vue'
import MyFooter from '@/components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter
  },
  data() {
    return {
      isWindowScroll: false
    }
  },
  mounted () {
    window.addEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll () {
      if ((window.scrollY) == 0) {
        //alert("you're at the bottom of the page");
        this.isWindowScroll = false;
      } else {
        this.isWindowScroll = true;
      }
    }
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
