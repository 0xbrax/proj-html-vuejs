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
                    <div class="team-card flex align-ctr mt-40" v-for="(team, teamIndex) in teamCard" :key="teamIndex">
                        <img :src="require(`@/assets/img/${team.imgPath}`)" :alt="team.name">

                        <div class="ml-20">
                            <h3>{{team.name}}</h3>
                            <div class="color-grey txt-up mt-20">{{team.title}}</div>
                            <div class="mt-20">
                                <a class="circle-back-alt" :href="team.facebook">
                                    <i class="fa-brands fa-facebook-f"></i>
                                </a>
                                <a class="circle-back-alt ml-20" :href="team.twitter">
                                    <i class="fa-brands fa-twitter"></i>
                                </a>
                                <a class="circle-back-alt ml-20" :href="team.linkedin">
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
    name: 'MySectionTeam',
    data() {
        return {
            teamCard: [
                {
                    name: 'David Cooper',
                    title: 'CTO & co-founder',
                    imgPath: 'team-1.jpg',
                    facebook: '#',
                    twitter: '#',
                    linkedin: '#'
                },
                {
                    name: 'Oliver Jones',
                    title: 'Chief procurement',
                    imgPath: 'team-3.jpg',
                    facebook: '#',
                    twitter: '#',
                    linkedin: '#'
                },
                {
                    name: 'Emma Lopez',
                    title: 'Chief marketing',
                    imgPath: 'team-2.jpg',
                    facebook: '#',
                    twitter: '#',
                    linkedin: '#'
                },
                {
                    name: 'T. Johnson',
                    title: 'CEO & president',
                    imgPath: 'team-4.jpg',
                    facebook: '#',
                    twitter: '#',
                    linkedin: '#'
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