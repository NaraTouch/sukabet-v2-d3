<template>
    <div>
        <section class="home-container-area">
            <div class="container-fluid container-fluid-override">
                <div class="clearfix">
                     <div class="col-lg-8  float-lg-right ">
                            <SlotsGameComponent />
                    </div>
                    <div class="col-lg-4 float-lg-lef border-right box-margin-top">
                        <TabWinner :isactive="active" />
                        <OnlinePlayer />
                        <PaymentMethod />
                    </div>
                </div>
                <div class="clearfix">
                    <div class="col-lg-12"> 
                        <FooterText :link="link" :test="linkTitle" :contect="contect" />
                        <Footer />
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    data() {
        return {
            components: {
                TabWinner: () => import("@/components/TabWinner"),
                OnlinePlayer: () => import("@/components/OnlinePlayer"),
                PaymentMethod: () => import("@/components/PaymentMethod"),
                Footer: () => import('@/components/Footer'),
                SlotsGameComponent: () => import('@/components/SlotsGameComponent'),
            },
             link: "http://localhost:3000/",
            contect: "Selamat datang di situs Sukabet situs dermainan online terlenakap dan terpercava. Pada halaman in anda dapat memilih kategori permainan vang anda inqin mainkan saat In. Bag andd yang Delum au, Dartar Can dapatkan DOnus pemain Daru di SituS Kami. Rasakan keservan yang relan dirasakan oleh pemain lainnya., Jangan ketingqalan permainan terbaru yanq seru di situs kami, Kami hanya memiliki permainan-permainan terbaik agar anda tidak binqund",
            linkTitle: "Baca selanjutnya",
            active: true,
        }
    },
}
</script>