<template>
    <section class="home-container-area">
        <div class="container-fluid">
            <div class="row">
                <div class="col-lg-3">
                    <TabWinner />
                    <OnlinePlayer />
                </div>
                <div class="col-lg-9">

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
        },
    };
</script>
