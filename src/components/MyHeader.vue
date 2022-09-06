<template>
    <header>
        <div class="topbar">
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

        <nav class="container flex align-ctr txt-up">
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
        </nav>
    </header>
</template>

<script>
export default {
    name: 'MyHeader',
    data() {
        return {
            headerLink: [
                {
                    url: '#',
                    name: 'Home'
                },
                {
                    url: '#',
                    name: 'About'
                },
                {
                    url: '#',
                    name: 'Services'
                },
                {
                    url: '#',
                    name: 'Process'
                },
                {
                    url: '#',
                    name: 'Team'
                },
                {
                    url: '#',
                    name: 'Blog'
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

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
    }

    .logo-main {
        width: 30%;
    }

    .logo-txt {
        display: inline-block;
        padding: 10px 20px;
        border-radius: 20px;
        background: linear-gradient(90deg, rgba(69, 186, 188, 0.3) 0%, rgba(69, 186, 188, 0.3) 48%, rgba(255,255,255,0) 48%);
    }

    .menu-main {
        width: 70%;

        li {
            display: inline-block;
        }
    }
</style>