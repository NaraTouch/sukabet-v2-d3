<template>
     <div class="mb-5-margin-bottom">
        <section class="payment-method box-shadow-1 border-raduis-10 bg-white">
            <div class="container pr-0 pl-0 mb-2">
                <div class="row mr-0 ml-0">
                    <div class="col-lg-12 pr-0 pl-0">
                        <div class="brand-logo-content size-game">
                            <div class="col-lg-2 col-md-3 col-sm-4 mb-3 col-xs-6 on-pl-col image-size" v-for="(brand, index) in brands" :key="index">
                                <div class="brand-logo-item">
                                    <img :src="brand.logoSrc" :alt="brand.alt">
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <FooterText :link="link" :test="linkTitle" :contect="contect" />
    </div>
</template>
<script>
export default {
    data() {
        return {
            brands: [
                    {
                        logoSrc: "/images/bank/images.jpg",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/images.jpg",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/images.jpg",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/images.jpg",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/images.jpg",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/images.jpg",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/images.jpg",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/images.jpg",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/images.jpg",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/images.jpg",
                        alt: "Brand Name"
                    },
                     {
                        logoSrc: "/images/bank/images.jpg",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/images.jpg",
                        alt: "Brand Name"
                    },
                ],
                link: "http://localhost:3000/",
                contect: "Selamat datang di situs Sukabet situs dermainan online terlenakap dan terpercava. Pada halaman in anda dapat memilih kategori permainan vang anda inqin mainkan saat In. Bag andd yang Delum au, Dartar Can dapatkan DOnus pemain Daru di SituS Kami. Rasakan keservan yang relan dirasakan oleh pemain lainnya., Jangan ketingqalan permainan terbaru yanq seru di situs kami, Kami hanya memiliki permainan-permainan terbaik agar anda tidak binqund",
                linkTitle: "Baca selanjutnya",
            }
    },
}
</script>