<template>
    <section>
        <div class="container">
            <div class="flex align-end">
                <div class="services">

                </div>
                <div>
                    button
                </div>
            </div>

            <div class="flex wrap">
                <!-- VUE CYCLE -->
                <div class="services-card">

                </div>
                <div class="services-card">

                </div>
                <div class="services-card">

                </div>
                <div class="services-card">

                </div>
                <div class="services-card">

                </div>
                <div class="services-card">

                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MySectionServices'
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    .services {
        width: 80%;
    }

    .services-card {
        width: calc(100% / 3);
    }
</style>