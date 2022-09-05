<template>
    <section>
        <div class="container flex align-end">
            <div class="team-card-container">
                <div class="team">

                </div>

                <div class="flex wrap">
                    <!-- VUE CYCLE -->
                    <div class="team-card">

                    </div>
                    <div class="team-card">

                    </div>
                    <div class="team-card">

                    </div>
                    <div class="team-card">

                    </div>
                </div>
            </div>

            <div>
                test card
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MySectionTeam'
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    .team-card-container {
        width: 70%;
    }

    .team-card {
        width: 50%;
    }
</style>