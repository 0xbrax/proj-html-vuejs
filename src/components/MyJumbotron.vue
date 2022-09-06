<template>
    <section>
        <div class="container flex just-end align-ctr">
            <div class="hero">
                <div class="txt-up txt-bold color-brand-dark">Fusions &amp; acquisitions</div>
                <h1>Insurance consulting</h1>

                <div class="flex wrap just-sp-bw">
                    <input class="mt-20" type="text" placeholder="Name">
                    <input class="mt-20" type="text" placeholder="Email">
                    <input class="mt-20" type="text" placeholder="Phone">
                    <select class="mt-20">
                        <option value="1">More info</option>
                    </select>
                </div>

                <a class="btn-main mt-20" href="#">Get in touch</a>
                <a class="btn-sec mt-20 ml-20" href="#">Read more</a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MyJumbotron'
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    section {
        background-image: url('@/assets/img/bg-6.jpg');
        background-position: center;
        height: 600px;
        margin-top: 110px;

        .container {
            height: 100%;
        }
    }

    .hero {
        width: 40%;
    }

    h1 {
        font-size: 50px;
    }

    input,
    select {
        width: 48%;
        padding: 10px;
        background-color: $grey-light;
        border: 0;
        border-radius: 5px;
    }
</style>