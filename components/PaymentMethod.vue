<template>
    <div class="mb-5">
        <section class="payment-method box-shadow-1 border-raduis-10 bg-white">
            <div class="container pr-0 pl-0 mb-2">
                <div class="row mr-0 ml-0">
                    <div class="col-12 pt-2 pb-2">
                        <div class="payment-head">
                            <span><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-credit-card" viewBox="0 0 16 16">
                              <path d="M0 4a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v8a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V4zm2-1a1 1 0 0 0-1 1v1h14V4a1 1 0 0 0-1-1H2zm13 4H1v5a1 1 0 0 0 1 1h12a1 1 0 0 0 1-1V7z"/>
                              <path d="M2 10a1 1 0 0 1 1-1h1a1 1 0 0 1 1 1v1a1 1 0 0 1-1 1H3a1 1 0 0 1-1-1v-1z"/>
                            </svg>  </span>
                            <span class="text-black">Payment Method</span>
                        </div>
                    </div>
                </div>
                <div class="row mr-0 ml-0" data-aos="fade-up" data-aos-duration="1000">
                    <div class="col-lg-12 pr-0 pl-0">
                        <div class="brand-logo-content">
                            <div class="col-3 mb-2 on-pl-col" v-for="(brand, index) in brands" :key="index">
                                <div class="brand-logo-item">
                                    <img :src="brand.logoSrc" :alt="brand.alt">
                                </div>
                            </div>
                        </div>
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
                brands: [
                    {
                        logoSrc: "/images/bank/aba.png",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/aba.png",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/aba.png",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/aba.png",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/aba.png",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/aba.png",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/aba.png",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/aba.png",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/aba.png",
                        alt: "Brand Name"
                    },
                    {
                        logoSrc: "/images/bank/aba.png",
                        alt: "Brand Name"
                    },
                ]
            }
        },
    };
</script>
