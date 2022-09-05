<template>
    <main>
        <MyJumbotron />
        <MySectionAbout />
        <MySectionServices />
        <MySectionProcess />
        <MySectionTeam />
        <MySectionBlog />
        <MySectionContact />
    </main>
</template>

<script>
import MyJumbotron from '@/components/MyJumbotron.vue'
import MySectionAbout from '@/components/MySectionAbout.vue'
import MySectionServices from '@/components/MySectionServices.vue'
import MySectionProcess from '@/components/MySectionProcess.vue'
import MySectionTeam from '@/components/MySectionTeam.vue'
import MySectionBlog from '@/components/MySectionBlog.vue'
import MySectionContact from '@/components/MySectionContact.vue'

export default {
    name: 'MyMain',
    components: {
        MyJumbotron,
        MySectionAbout,
        MySectionServices,
        MySectionProcess,
        MySectionTeam,
        MySectionBlog,
        MySectionContact
    }
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

</style>