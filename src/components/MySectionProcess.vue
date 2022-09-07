<template>
    <section id="process-id" class="py-120 txt-ctr">
        <div>
            <div class="process">
                <div class="container">
                    <div class="color-brand-dark txt-up txt-bold">How it works in pratice</div>
                    <h2 class="mt-20"><span class="band-tag-back color-brand-dark">Process</span> Management</h2>
                    <p class="color-grey mt-20">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto laudantium laborum, mollitia ullam, explicabo recusandae commodi iste id expedita aut sequi necessitatibus.</p>
                </div>
            </div>

            <div class="process-card-container mt-40">
                <div class="process-card-fx"></div>

                <div class="container-large flex wrap just-sp-bw">
                    <div class="process-card" v-for="(process, processIndex) in processCard" :key="processIndex">
                    <span class="circle-back">{{process.number}}</span>
                    <h4 class="mt-20">{{process.title}}</h4>
                    <p class="color-grey mt-20">{{process.overview}}</p>
                </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MySectionProcess',
    data() {
        return {
            processCard: [
                {
                    number: '01',
                    title: 'Collection of information',
                    overview: 'Lorem ipsum dolor sit amet consectetur'
                },{
                    number: '02',
                    title: 'Strategic planning',
                    overview: 'Lorem ipsum dolor sit amet consectetur'
                },
                {
                    number: '03',
                    title: 'Assignment of responsibilities',
                    overview: 'Lorem ipsum dolor sit amet consectetur'
                },
                {
                    number: '04',
                    title: 'Formatting process',
                    overview: 'Lorem ipsum dolor sit amet consectetur'
                },
                {
                    number: '05',
                    title: 'Continuity formalization',
                    overview: 'Lorem ipsum dolor sit amet consectetur'
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';

    .process {
        .container {
            width: 50%;
        }
    }

    .process-card-container {
        position: relative;
    }

    .process-card-fx {
        height: 4px;
        width: 100%;
        background-color:rgba(4, 131, 131, 0.2);
        position: absolute;
        top: 18px;
        left: 50%;
        transform: translateX(-50%);
        z-index: 1;
    }

    .process-card {
        width: calc(91% / 5);
        position: relative;
        z-index: 2;
    }
</style>