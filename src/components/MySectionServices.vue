<template>
    <section id="services-id" class="py-120">
        <div class="container">
            <div class="flex just-sp-bw align-end">
                <div class="services">
                    <div class="color-brand-dark txt-up txt-bold">Our business areas</div>
                    <h2 class="mt-20">Excellence in <span class="band-tag-back color-brand-dark">Services</span></h2>
                    <p class="color-grey mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto laudantium laborum, mollitia ullam, explicabo recusandae commodi iste id expedita aut sequi necessitatibus, adipisci tenetur porro ea consectetur?</p>
                </div>
                <div>
                    <a class="btn-main" href="#">See all</a>
                </div>
            </div>

            <div class="flex wrap just-sp-bw mt-20">
                <div class="services-card mt-20" v-for="(services, servicesIndex) in servicesCard" :key="servicesIndex">
                    <div class="flex just-sp-bw">
                        <i class="color-brand-dark font-s30" :class="services.icon"></i>
                        <i class="fa-solid fa-arrow-right color-brand-light"></i>
                    </div>
                    <h4 class="mt-20">{{services.name}}</h4>
                    <p class="color-grey mt-20">{{services.overview}}</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MySectionServices',
    data() {
        return {
            servicesCard: [
                {
                    icon: 'fa-solid fa-network-wired',
                    name: 'Audit & Assurance',
                    overview: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit.'
                },
                {
                    icon: 'fa-solid fa-briefcase',
                    name: 'Financial Advisory',
                    overview: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit.'
                },
                {
                    icon: 'fa-solid fa-chart-simple',
                    name: 'Analytics and M&A',
                    overview: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit.'
                },
                {
                    icon: 'fa-solid fa-plane',
                    name: 'Middle Marketing',
                    overview: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit.'
                },
                {
                    icon: 'fa-solid fa-magnifying-glass',
                    name: 'Legal Consulting',
                    overview: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit.'
                },
                {
                    icon: 'fa-solid fa-box',
                    name: 'Regulatory Risk',
                    overview: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit.'
                }
            ],
        }
    }
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    section {
        background-color: $black-haze;
    }

    .services {
        width: 80%;
    }

    .services-card {
        width: calc(94% / 3);
        padding: 20px;
        background-color: $white;
        border-radius: 5px;
    }
</style>