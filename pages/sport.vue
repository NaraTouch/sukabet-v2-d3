<template>
    <div class="home-default-wrapper">

        <Header />
        <RunningText />
        <div class="container bg-gray-lighter">
            <OffCanvasMobileMenu />
            <SportContainer />
            <!-- <BaccaratContainer /> -->
            
<!--            <HeroOne />-->

<!--            <ServiceOne />-->

<!--            <CausesOne />-->

<!--            <FunFactOne />-->

<!--            <Sponsor />-->

            <client-only>
                <back-to-top class="scroll-top" bottom="30px">
                    <i class="arrow-top icofont-rounded-up"></i>
                    <i class="arrow-bottom icofont-rounded-up"></i>
                </back-to-top>
            </client-only>
        </div>
        
        <!-- <Footer /> -->
    </div>
</template>

<script>
    export default {
        components: {
            Header: () => import('@/components/Header'),
            OffCanvasMobileMenu: () => import('@/components/OffCanvasMobileMenu'),
            Breadcrumb: () => import('@/components/Breadcrumb'),
            PricingWrapper: () => import('@/components/PricingWrapper'),
            SportContainer: () => import('@/components/Sport/SportContainer'),
            // Footer: () => import('@/components/Footer'),
        },

        data() {
            return {
                items: [
                    {
                        text: 'Home',
                        to: "/"
                    },
                    {
                        text: 'sport',
                        active: true
                    }
                ]
            }
        },

        head() {
            return {
                title: 'Sport'
            }
        },
    };
</script>


