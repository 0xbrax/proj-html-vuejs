<template>
    <footer>
        <div class="bottombar py-120">
            <div class="container flex just-sp-bw">
                <div class="info-card">
                    <div class="logo-txt txt-space txt-bold txt-up">
                        <span class="color-brand-dark">Nex</span><span class="color-white">gen</span>
                    </div>
                    <p class="mt-40">A Functional HTML Template for Corporate &amp; Business.</p>
                    <div class="mt-20"><i class="fa-solid fa-phone"></i> +1 (305) 1234-5678</div>
                    <div class="mt-20"><i class="fa-solid fa-envelope"></i> hello@example.com</div>
                    <div class="mt-20"><i class="fa-solid fa-location-dot"></i> Main Avenue, 987</div>
                    <a class="btn-sec mt-40" href="#">Get in touch</a>
                </div>

                <div class="info-card card-special" v-for="(info, infoIndex) in infoCard" :key="infoIndex">
                    <h3 class="color-white">{{info.category}}</h3>
                    <div class="mt-20" v-for="(link, linkIndex) in info.links" :key="linkIndex">
                        <div class="mt-20">
                            <i class="fa-solid fa-angle-right"></i> <a :href="link.url">{{link.name}}</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="foot-bottom font-s14">
            <div class="container flex">
            <div class="credits">
                Enjoy the low price. We are tracking any intention of piracy.
            </div>
            <div class="credits txt-r">
                &copy; <span class="txt-up">Nexgen</span> is Proudly Powered by <a href="#" class="color-brand-dark">Codings</a>.
            </div>
        </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'MyFooter',
    data() {
        return {
            infoCard: [
                {
                    category: 'About',
                    links: [
                        {
                            url: '#',
                            name: 'The company'
                        },
                        {
                            url: '#',
                            name: 'Institutional'
                        },
                        {
                            url: '#',
                            name: 'Social & Events'
                        },
                        {
                            url: '#',
                            name: 'Innovation'
                        },
                        {
                            url: '#',
                            name: 'Environment'
                        },
                        {
                            url: '#',
                            name: 'Technology'
                        }
                    ]
                },
                {
                    category: 'Services',
                    links: [
                        {
                            url: '#',
                            name: 'The company'
                        },
                        {
                            url: '#',
                            name: 'Institutional'
                        },
                        {
                            url: '#',
                            name: 'Social & Events'
                        },
                        {
                            url: '#',
                            name: 'Innovation'
                        },
                        {
                            url: '#',
                            name: 'Environment'
                        },
                        {
                            url: '#',
                            name: 'Technology'
                        }
                    ]
                },
                {
                    category: 'Support',
                    links: [
                        {
                            url: '#',
                            name: 'The company'
                        },
                        {
                            url: '#',
                            name: 'Institutional'
                        },
                        {
                            url: '#',
                            name: 'Social & Events'
                        },
                        {
                            url: '#',
                            name: 'Innovation'
                        },
                        {
                            url: '#',
                            name: 'Environment'
                        },
                        {
                            url: '#',
                            name: 'Technology'
                        }
                    ]
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    footer {
        color: $cloudy;
    }

    .bottombar {
        background-color: $black-var;
    }

    .info-card {
        width: calc(91% / 4);
    }

    a {
        color: $white;
    }

    .card-special {
        background-color: rgba(165, 160, 157, 0.3);
        border-radius: 10px;
        padding: 30px;

        a {
            color: $cloudy;
        }
    }

        .foot-bottom {
            background-color: #000000;
            padding: 30px 0;
        }

    .credits {
        width: 50%;
    }
</style>