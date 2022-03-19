<template>
   <div>
        <section class="home-container-area">
            <div class="container-fluid container-fluid-override">
                <div class="clearfix">
                     <div class="col-lg-8 float-lg-right">
                        <BaccaratGame :game-link="baccaratGames"/>
                    </div>
                    <div class="col-lg-4 float-lg-left border-right box-margin-top">
                        <TabWinner />
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
                BaccaratGame: () => import('@/components/BaccaratGame'),
                FooterText: () => import('@/components/footer-text'),
            },
            link: "http://localhost:3000/",
            contect: "Selamat datang di situs Sukabet situs dermainan online terlenakap dan terpercava. Pada halaman in anda dapat memilih kategori permainan vang anda inqin mainkan saat In. Bag andd yang Delum au, Dartar Can dapatkan DOnus pemain Daru di SituS Kami. Rasakan keservan yang relan dirasakan oleh pemain lainnya., Jangan ketingqalan permainan terbaru yanq seru di situs kami, Kami hanya memiliki permainan-permainan terbaik agar anda tidak binqund",
            linkTitle: "Baca selanjutnya",
            baccaratGames: [
                { 
                    id: 1,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 2,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 3,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 4,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                }
            ]
        }
    },
}
</script>