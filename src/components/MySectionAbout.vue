<template>
    <section>
        <div class="container flex">
            <div class="about">

            </div>
            <div class="flex wrap">
                <!-- VUE CYCLE -->
                <div class="about-card">

                </div>
                <div class="about-card">

                </div>
                <div class="about-card">

                </div>
                <div class="about-card">

                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MySectionAbout'
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    .container > div,
    .about-card {
        width: 50%;
    }
</style>