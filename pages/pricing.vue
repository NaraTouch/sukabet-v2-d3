<template>
    <!-- <div class="main-container">

        <Header />

        <OffCanvasMobileMenu />

        <Breadcrumb :items="items" title="Pricing" />

        <PricingWrapper />

        <Footer />

        <client-only>
            <back-to-top class="scroll-top" bottom="30px">
                <i class="arrow-top icofont-rounded-up"></i>
                <i class="arrow-bottom icofont-rounded-up"></i>
            </back-to-top>
        </client-only>

    </div> -->
    <div class="home-default-wrapper">

        <Header />
        <RunningText />
        <ActionComponent />
        <div class="container bg-gray-lighter">
            <OffCanvasMobileMenu />
            <BaccaratContainer />
            
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
            BaccaratContainer: () => import('@/components/Baccarat/BaccaratContainer'),
            ActionComponent: () => import('@/components/Home/ActionComponent'),
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
                        text: 'pricing',
                        active: true
                    }
                ]
            }
        },

        head() {
            return {
                title: 'Pricing'
            }
        },
    };
</script>


