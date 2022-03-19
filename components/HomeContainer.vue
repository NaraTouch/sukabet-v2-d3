<template>
    <section class="home-container-area">
        <div class="container-fluid container-fluid-override">
            <div class="clearfix">
                <div class="col-lg-8 float-lg-right">
                     <SlideBar :images="imageLink"/>
                </div>
                <div class="col-lg-4 float-lg-left border-right box-margin-top ">
                    <div v-if="isActive" class="new-hot-offer">
                         <div></div>
                    </div>
                    <TabWinner />
                    <OnlinePlayer />
                    <PaymentMethod />
                </div>
                <div class="col-lg-8 float-lg-right col-margin-top">
                    <CardGameList />
                </div>
            </div>
            <div class="clearfix">
                 <div class="col-lg-12"> 
                    <MoreGame />
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                components: {
                    TabWinner: () => import("@/components/TabWinner"),
                    OnlinePlayer: () => import("@/components/OnlinePlayer"),
                    PaymentMethod: () => import("@/components/PaymentMethod"),
                    SlideBar: () => import('@/components/SlideBar'),
                    CardGameList: () => import('@/components/CardGameList'),
                    MoreGame: () => import('@/components/MoreGame.vue'),
                },
                imageLink: [
                    {
                        id: 1, 
                        src: require('../static/images/slide-bar-image/image-1.jpg')
                    },
                    {
                        id: 2,
                        src: require('../static/images/slide-bar-image/image-2.jpg')
                    },
                ],
                isActive: true,
            }
        },
    };
</script>
