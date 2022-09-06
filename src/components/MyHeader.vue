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
            <div class="container flex align-ctr txt-up">
                <div class="logo-main">
                    <div class="logo-txt">
                        <a class="txt-space txt-bold" href="#"><span class="color-brand-dark">Nex</span><span class="color-black">gen</span></a>
                    </div>
                </div>

                <div class="menu-main txt-r">
                    <ul>
                        <li v-for="(link, linkIndex) in headerLink" :key="linkIndex" class="ml-20"><a :href="link.url">{{link.name}}</a></li>
                        <li class="ml-20"><a class="btn-main" href="#">Get in touch</a></li>
                    </ul>
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
            ]
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
        width: 30%;
    }

    .logo-txt {
        display: inline-block;
        padding: 10px 20px;
        border-radius: 20px;
        background: linear-gradient(90deg, rgba(4, 131, 131, 0.2) 0%, rgba(4, 131, 131, 0.2) 48%, rgba(255,255,255,0) 48%);
    }

    .menu-main {
        width: 70%;

        li {
            display: inline-block;
        }
    }
</style>