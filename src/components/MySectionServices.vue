<template>
    <section class="py-120">
        <div class="container">
            <div class="flex just-sp-bw align-end">
                <div class="services">
                    <div class="color-brand-dark txt-up txt-bold">Our business areas</div>
                    <h2 class="mt-20">Excellence in <span class="band-tag-back color-brand-dark">Services</span></h2>
                    <p class="mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto laudantium laborum, mollitia ullam, explicabo recusandae commodi iste id expedita aut sequi necessitatibus, adipisci tenetur porro ea consectetur?</p>
                </div>
                <div>
                    <a class="btn-main" href="#">See all</a>
                </div>
            </div>

            <div class="flex wrap just-sp-bw">
                <div class="services-card mt-20">
                    <div class="flex just-sp-bw">
                        <i class="fa-solid fa-network-wired color-brand-dark font-s30"></i>
                        <i class="fa-solid fa-arrow-right color-brand-light"></i>
                    </div>
                    <h4 class="mt-20">Audit &amp; Assurance</h4>
                    <p class="mt-20">Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
                </div>

                <div class="services-card mt-20">
                    <div class="flex just-sp-bw">
                        <i class="fa-solid fa-briefcase color-brand-dark font-s30"></i>
                        <i class="fa-solid fa-arrow-right color-brand-light"></i>
                    </div>
                    <h4 class="mt-20">Financial Advisory</h4>
                    <p class="mt-20">Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
                </div>

                <div class="services-card mt-20">
                    <div class="flex just-sp-bw">
                        <i class="fa-solid fa-chart-simple color-brand-dark font-s30"></i>
                        <i class="fa-solid fa-arrow-right color-brand-light"></i>
                    </div>
                    <h4 class="mt-20">Analytics and M&amp;A</h4>
                    <p class="mt-20">Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
                </div>

                <div class="services-card mt-20">
                    <div class="flex just-sp-bw">
                        <i class="fa-solid fa-plane fa-rotate-by color-brand-dark font-s30" style="--fa-rotate-angle: 315deg;"></i>
                        <i class="fa-solid fa-arrow-right color-brand-light"></i>
                    </div>
                    <h4 class="mt-20">Middle Marketing</h4>
                    <p class="mt-20">Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
                </div>

                <div class="services-card mt-20">
                    <div class="flex just-sp-bw">
                        <i class="fa-solid fa-magnifying-glass color-brand-dark font-s30"></i>
                        <i class="fa-solid fa-arrow-right color-brand-light"></i>
                    </div>
                    <h4 class="mt-20">Legal Consulting</h4>
                    <p class="mt-20">Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
                </div>

                <div class="services-card mt-20">
                    <div class="flex just-sp-bw">
                        <i class="fa-solid fa-box color-brand-dark font-s30"></i>
                        <i class="fa-solid fa-arrow-right color-brand-light"></i>
                    </div>
                    <h4 class="mt-20">Regulatory Risk</h4>
                    <p class="mt-20">Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
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