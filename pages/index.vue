<template>
    <div class="home-default-wrapper">
        <Header />
        <RunningText />
        <ActionComponent />
        <div class="container bg-gray-lighter">
            <OffCanvasMobileMenu />
            <HomeContainer />
            
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
        
        <Footer />
    </div>
</template>

<script>
    export default {
        components: {
            Header: () => import('@/components/Header'),
            RunningText: () => import('@/components/RunningText'),
            OffCanvasMobileMenu: () => import('@/components/OffCanvasMobileMenu'),
            HomeContainer: () => import('@/components/HomeContainer'),
            ActionComponent: () => import('@/components/Home/ActionComponent'),
            // HeroOne: () => import('@/components/HeroOne'),
            // ServiceOne: () => import('@/components/ServiceOne'),
            // CausesOne: () => import('@/components/CausesOne'),
            // FunFactOne: () => import('@/components/FunFactOne'),
            // Sponsor: () => import('@/components/Sponsor'),
            // Footer: () => import('@/components/Footer'),
        },

        head() {
            return {
                title: 'Home',
            }
        },
    };
</script>


