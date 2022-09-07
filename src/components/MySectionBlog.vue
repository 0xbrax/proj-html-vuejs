<template>
    <section class="py-120">
        <div class="container">
            <div class="flex just-sp-bw align-end">
                <div class="blog">
                    <div class="color-brand-dark txt-up txt-bold">Our editorial content</div>
                    <h2 class="mt-20"><span class="band-tag-back color-brand-dark">Lastest</span> News</h2>
                    <p class="mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto laudantium laborum, mollitia ullam.</p>
                </div>
                <div>
                    <a class="btn-main" href="#">See all</a>
                </div>
            </div>

            <div class="flex just-sp-bw mt-40 flex">
                <div class="blog-card" v-for="(blog, blogIndex) in blogCard" :key="blogIndex">
                    <img :src="require(`@/assets/img/${blog.imgPath}`)" :alt="blog.overview">
                    <div class="img-overlay flex align-end txt-bold txt-ctr">
                        {{blog.overview}}
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MySectionBlog',
    data() {
        return {
            blogCard: [
                {
                    imgPath: 'news-1.jpg',
                    overview: 'Increasing creativity is possible for everyone'
                },
                {
                    imgPath: 'news-2.jpg',
                    overview: 'Because market research is part of the business plan'
                },
                {
                    imgPath: 'news-3.jpg',
                    overview: 'Working from home is now a trend'
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    .blog {
        width: 80%;
    }

    .blog-card {
        width: calc(94% / 3);
        aspect-ratio: 1 / 1;
        border-radius: 10px;
        overflow: hidden;
        position: relative;

        img {
            width: 100%;
        }

        .img-overlay {
            width: 100%;
            height: 100%;
            position: absolute;
            bottom: 0;
            color: $white;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px 30px;
            font-size: 20px;
        }
    }
</style>