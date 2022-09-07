<template>
    <header>
        <div class="topbar font-s14" v-if="checkScroll == false">
            <div class="container flex just-sp-bw align-ctr">
                <div class="topbar-l">
                    <i class="fa-solid fa-clock"></i> Open Hours: Mon - Sat / 9:00 - 18:00
                </div>

                <div class="topbar-r txt-r">
                    <span>
                        <i class="fa-solid fa-phone"></i> +1 (305) 1234-5678
                    </span>
                    <span class="ml-20">
                        <i class="fa-solid fa-envelope"></i> hello@example.com
                    </span>

                    <a class="ml-20" href="#">
                        <i class="fa-brands fa-facebook-f"></i>
                    </a>
                    <a class="ml-20" href="#">
                        <i class="fa-brands fa-twitter"></i>
                    </a>
                    <a class="ml-20" href="#">
                        <i class="fa-brands fa-linkedin-in"></i>
                    </a>
                </div>
            </div>
        </div>

        <nav>
            <div class="container flex just-sp-bw align-ctr txt-up">
                <div class="logo-main">
                    <div class="logo-txt">
                        <a class="txt-space txt-bold" href="#"><span class="color-brand-dark">Nex</span><span class="color-black">gen</span></a>
                    </div>
                </div>

                <div class="menu-main flex just-end align-ctr">
                    <div class="menu-list flex">
                        <a v-for="(link, linkIndex) in headerLink" :key="linkIndex" class="color-black" :class="linkIndex == whoIsSelected ? 'active' : ''"
                        :href="link.url" @click="setLinkActive(linkIndex)">
                            {{link.name}}
                        </a>
                    </div>
                    <a class="btn-main ml-10" href="#contact-id">Get in touch</a>
                </div>
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'MyHeader',
    props: {
        checkScroll: Boolean
    },
    data() {
        return {
            headerLink: [
                {
                    url: '#',
                    name: 'Home'
                },
                {
                    url: '#about-id',
                    name: 'About'
                },
                {
                    url: '#services-id',
                    name: 'Services'
                },
                {
                    url: '#process-id',
                    name: 'Process'
                },
                {
                    url: '#team-id',
                    name: 'Team'
                },
                {
                    url: '#blog-id',
                    name: 'Blog'
                }
            ],
            whoIsSelected: 0
        }
    },
    methods: {
        setLinkActive(index) {
            this.whoIsSelected = index;
        }
    }
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    header {
        position: fixed;
        z-index: 999;
        top: 0;
        width: 100%;
    }

    .topbar {
        height: 40px;
        color: $black-haze;
        background-color: $limed-spruce;

        .container {
            height: 100%;
        }

        a {
            color: $black-haze;
        }
    }

    .topbar-l {
        width: 30%;
    }
    .topbar-r {
        width: 70%;
    }

    nav {
        height: 70px;
        background-color: $white;

        .container {
            height: 100%;
        }
    }

    .logo-main {
        width: 20%;
    }

    .menu-main {
        width: 80%;
        height: 100%;

        .menu-list {
            height: 100%;

            a {
                line-height: 70px;
                height: 100%;
                padding: 0 10px;

                &:hover {
                    background-color: rgba(4, 131, 131, 0.1);
                    box-shadow: inset 0px -5px 0px 0px $brand-color-dark;
                }
            }
        }
    }
</style>