<template>
    <section>
        <div class="container">
            <div class="flex align-end">
                <div class="blog">

                </div>
                <div>
                    button
                </div>
            </div>

            <div class="flex">
                <!-- VUE CYCLE -->
                <div class="blog-card">

                </div>
                <div class="blog-card">

                </div>
                <div class="blog-card">

                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MySectionBlog'
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    .blog {
        width: 80%;
    }

    .blog-card {
        width: calc(100% / 3);
    }
</style>