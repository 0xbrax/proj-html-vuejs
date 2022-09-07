<template>
    <section id="team-id" class="py-120">
        <div class="container flex just-sp-bw align-end">
            <div class="team-card-container">
                <div class="team">
                    <div class="color-brand-dark txt-up txt-bold">About the network</div>
                    <h2 class="mt-20"><span class="band-tag-back">Team</span> of Experts</h2>
                    <p class="color-grey mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto laudantium laborum, mollitia ullam, explicabo recusandae commodi iste id expedita aut sequi necessitatibus.</p>
                </div>

                <div class="flex wrap just-sp-bw">
                    <div class="team-card flex align-ctr mt-40">
                        <img src="@/assets/img/team-1.jpg" alt="David Cooper">

                        <div class="ml-20">
                            <h3>David Cooper</h3>
                            <div class="color-grey txt-up mt-20">CTO &amp; co-founder</div>
                            <div class="mt-20">
                                <a class="circle-back-alt" href="#">
                                    <i class="fa-brands fa-facebook-f"></i>
                                </a>
                                <a class="circle-back-alt ml-20" href="#">
                                    <i class="fa-brands fa-twitter"></i>
                                </a>
                                <a class="circle-back-alt ml-20" href="#">
                                    <i class="fa-brands fa-linkedin-in"></i>
                                </a>
                            </div>
                        </div>
                    </div>

                    <div class="team-card flex align-ctr mt-40">
                        <img src="@/assets/img/team-3.jpg" alt="Oliver Jones">

                        <div class="ml-20">
                            <h3>Oliver Jones</h3>
                            <div class="color-grey txt-up mt-20">Chief procurement</div>
                            <div class="mt-20">
                                <a class="circle-back-alt" href="#">
                                    <i class="fa-brands fa-facebook-f"></i>
                                </a>
                                <a class="circle-back-alt ml-20" href="#">
                                    <i class="fa-brands fa-twitter"></i>
                                </a>
                                <a class="circle-back-alt ml-20" href="#">
                                    <i class="fa-brands fa-linkedin-in"></i>
                                </a>
                            </div>
                        </div>
                    </div>

                    <div class="team-card flex align-ctr mt-40">
                        <img src="@/assets/img/team-2.jpg" alt="emma Lopez">

                        <div class="ml-20">
                            <h3>Emma Lopez</h3>
                            <div class="color-grey txt-up mt-20">Chief marketing</div>
                            <div class="mt-20">
                                <a class="circle-back-alt" href="#">
                                    <i class="fa-brands fa-facebook-f"></i>
                                </a>
                                <a class="circle-back-alt ml-20" href="#">
                                    <i class="fa-brands fa-twitter"></i>
                                </a>
                                <a class="circle-back-alt ml-20" href="#">
                                    <i class="fa-brands fa-linkedin-in"></i>
                                </a>
                            </div>
                        </div>
                    </div>

                    <div class="team-card flex align-ctr mt-40">
                        <img src="@/assets/img/team-4.jpg" alt="T. Johnson">

                        <div class="ml-20">
                            <h3>T. Johnson</h3>
                            <div class="color-grey txt-up mt-20">CEO &amp; president</div>
                            <div class="mt-20">
                                <a class="circle-back-alt" href="#">
                                    <i class="fa-brands fa-facebook-f"></i>
                                </a>
                                <a class="circle-back-alt ml-20" href="#">
                                    <i class="fa-brands fa-twitter"></i>
                                </a>
                                <a class="circle-back-alt ml-20" href="#">
                                    <i class="fa-brands fa-linkedin-in"></i>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="team-card-info">
                <h4>President Speech</h4>
                <p class="color-brand-alt-light mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                <p class="color-brand-alt-light mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto ratione quidem voluptates!</p>
                <p class="color-brand-alt-light mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                <div class="flex just-sp-bw align-ctr mt-20">
                    <h4>T. Johnson</h4>
                    <i class="fa-solid fa-quote-right fa-lg color-brand-alt-dark"></i>
                </div>
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

    section {
        background-color: $black-var;
        color: $white;
    }

    .team-card-container {
        width: 66%;
    }
    .team-card-info {
        width: 26%;
        background-color: $brand-color-dark;
        padding: 30px;
        border-radius: 5px;
    }

    .team-card {
        width: 48%;

        img {
            width: 30%;
            border-radius: 5px;
        }

        a {
            color: $brand-color-dark;
        }
    }
</style>