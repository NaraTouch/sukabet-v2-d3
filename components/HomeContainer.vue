<template>
    <section class="home-container-area">
        <div class="container-fluid">
            <div class="row">
                <div class="col-lg-4">
                    <TabWinner />
                    <OnlinePlayer />
                    <PaymentMethod />
                </div>
                <div class="col-lg-8">

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
        },
    };
</script>
