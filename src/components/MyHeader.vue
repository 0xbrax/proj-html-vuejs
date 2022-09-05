<template>
    <header>
        <div class="container">
            <div class="topbar flex">
                <div>

                </div>
                <div>

                </div>
            </div>

            <nav class="flex">
                <div class="logo-main">

                </div>

                <div class="menu-main">

                </div>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'MyHeader'
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    .logo-main {
        width: 30%;
    }

    .menu-main {
        width: 70%;
    }

    .topbar > div {
        width: 50%;
    }
</style>