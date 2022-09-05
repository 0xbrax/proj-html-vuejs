<template>
    <section>
        <div class="container">
            <div class="flex just-ctr">
                <div class="process">

                </div>
            </div>

            <div class="flex wrap">
                <!-- VUE CYCLE -->
                <div class="process-card">

                </div>
                <div class="process-card">

                </div>
                <div class="process-card">

                </div>
                <div class="process-card">

                </div>
                <div class="process-card">

                </div>
                <div class="process-card">

                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MySectionProcess'
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    .process {
        width: 60%;
    }

    .process-card {
        width: calc(100% / 6);
    }
</style>