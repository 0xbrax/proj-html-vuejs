<template>
    <section id="about-id" class="py-120">
        <div class="container flex just-sp-bw align-ctr">
            <div class="about">
                <div class="color-brand-dark txt-up txt-bold">About the network</div>
                <h2 class="mt-20"><span class="band-tag-back">The</span> Company</h2>
                <p class="mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto laudantium laborum, mollitia ullam, explicabo recusandae commodi iste id expedita aut sequi necessitatibus, adipisci tenetur porro ea consectetur? Veniam, neque earum.</p>
                <p class="mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit quidem expedita nisi cumque fugit corporis molestias qui minus, excepturi iusto!</p>
            </div>
            <div class="flex wrap just-sp-bw">
                <div class="about-card">
                    <div><i class="fa-solid fa-award color-brand-dark"></i> Tradition</div>
                    <p class="mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, omnis.</p>
                </div>
                <div class="about-card">
                    <div><i class="fa-solid fa-lock color-brand-dark"></i> Security</div>
                    <p class="mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, omnis.</p>
                </div>
                <div class="about-card mt-40">
                    <div><i class="fa-solid fa-pen-to-square color-brand-dark"></i> Certificate</div>
                    <p class="mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, omnis.</p>
                </div>
                <div class="about-card mt-40">
                    <div><i class="fa-solid fa-graduation-cap color-brand-dark"></i> Expertise</div>
                    <p class="mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, omnis.</p>
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

    section {
        background-color: $black-var;
        color: $white;
    }

    .container > div,
    .about-card {
        width: 46%;
    }
</style>