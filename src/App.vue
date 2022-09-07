<template>
  <div id="app">
    <MyHeader :checkScroll="isWindowScroll" />
    <MyMain />
    <MyFooter :checkGoTop="showGoToTop" />
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
      isWindowScroll: false,
      showGoToTop: false
    }
  },
  mounted () {
    window.addEventListener('scroll', () => {
      this.handleScroll();
      this.endScroll();
    });
    this.scrollSpy();
  },
  methods: {
    handleScroll() {
      if ((window.scrollY) == 0) {
        this.isWindowScroll = false;
      } else {
        this.isWindowScroll = true;
      }
    },
    endScroll() {
      if ((window.innerHeight + window.scrollY) >= document.body.scrollHeight) {
        this.showGoToTop = true;
      } else {
        this.showGoToTop = false;
      }
    },
    scrollSpy() {
      window.onscroll = (()=> {
        let menuSection = document.querySelectorAll('.menu-list a');
        let mainSection = document.querySelectorAll('section');

        menuSection.forEach(v=> {
          v.onclick = (()=> {
          setTimeout(()=> {
            menuSection.forEach(j=> j.classList.remove('active'))
            v.classList.add('active')
          },300)
          })
        })

        mainSection.forEach((v,i)=> {
          let rect = v.getBoundingClientRect().y
          if(rect < window.innerHeight-300){
            menuSection.forEach(v=> v.classList.remove('active'))
            menuSection[i].classList.add('active')
          }
        })
      })
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
