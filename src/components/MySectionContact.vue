<template>
    <section class="py-120">
        <div class="container">
            <div class="flex">
                <div class="contact">
                    <div class="color-brand-dark txt-up txt-bold">Newsletter</div>
                    <h2 class="mt-20"><span class="band-tag-back">Know</span> First</h2>
                    <p class="mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto laudantium laborum, mollitia ullam.</p>
                </div>

                <div class="contact">
                    <input type="text" placeholder="Name">
                    <input class="mt-20" type="text" placeholder="Email">
                    <a class="btn-main mt-20" href="#">Subscribe</a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MySectionContact'
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    section {
        background-image: url('@/assets/img/bg-1.jpg');
        background-position: center;
    }

    .contact {
        width: 48%;
        color: $white
    }

    input{
        width: 100%;
        padding: 10px;
        background-color: $white;
        opacity: 0.7;
        border: 0;
        border-radius: 5px;
    }
</style>