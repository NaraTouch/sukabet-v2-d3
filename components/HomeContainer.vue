<template>
    <section class="home-container-area">
        <div class="container-fluid">
            <div class="row">
                <div class="col-lg-4 border-right border-dark  box-margin-top">
                    <TabWinner />
                    <OnlinePlayer />
                    <PaymentMethod />
                </div>
                <div class="col-lg-8">
                    <SlideBar />
                    <CardGameList />
                </div>
                <div class="col-lg-12"> 
                    <MoreGame />
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        components: {
            TabWinner: () => import("@/components/TabWinner"),
            OnlinePlayer: () => import("@/components/OnlinePlayer"),
            PaymentMethod: () => import("@/components/PaymentMethod"),
            SlideBar: () => import('@/components/SlideBar'),
            CardGameList: () => import('@/components/CardGameList'),
            MoreGame: () => import('@/components/MoreGame.vue'),
        },
    };
</script>
