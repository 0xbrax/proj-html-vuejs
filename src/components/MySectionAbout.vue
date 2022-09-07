<template>
    <section id="about-id" class="py-120">
        <div class="container flex just-sp-bw align-ctr">
            <div class="about">
                <div class="color-brand-dark txt-up txt-bold">About the network</div>
                <h2 class="mt-20"><span class="band-tag-back">The</span> Company</h2>
                <p class="color-grey mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto laudantium laborum, mollitia ullam, explicabo recusandae commodi iste id expedita aut sequi necessitatibus, adipisci tenetur porro ea consectetur? Veniam, neque earum.</p>
                <p class="color-grey mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit quidem expedita nisi cumque fugit corporis molestias qui minus, excepturi iusto!</p>
            </div>

            <div class="flex wrap just-sp-bw">
                <div class="about-card mt-40" v-for="(about, aboutIndex) in aboutCard" :key="aboutIndex">
                    <div><i class="color-brand-dark" :class="about.icon"></i> {{about.name}}</div>
                    <p class="color-grey mt-20">{{about.overview}}</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MySectionAbout',
    data() {
        return {
            aboutCard: [
                {
                    icon: 'fa-solid fa-award',
                    name: 'Tradition',
                    overview: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, omnis.'
                },
                {
                    icon: 'fa-solid fa-lock',
                    name: 'Security',
                    overview: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, omnis.'
                },
                {
                    icon: 'fa-solid fa-pen-to-square',
                    name: 'Certificate',
                    overview: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, omnis.'
                },
                {
                    icon: 'fa-solid fa-graduation-cap',
                    name: 'Expertise',
                    overview: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, omnis.'
                }
            ],
        }
    }
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