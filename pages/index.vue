<template>
    <div class="home-default-wrapper">
        <Header />
        <RunningText />
        <ActionComponent />
        <!-- <div class="main-title">
            <a class="icon-image" target="_blank" href="#"><img :src="image"></a>
        </div> -->
        <DialogComponent>
            <template #slot-title>
               <!-- <h3>Hello world</h3> -->
                <!-- <div class="main-title">
                    <div class="icon-size">
                        <a class="icon-image" target="_blank" href="#"><img :src="image"></a>
                    </div>
                </div> -->
                <div class="border-radius">
                    <div class="icon-size">
                        <img :src="image" alt="" srcset="">
                    </div>
                </div>
            </template>
            <template #slot-body>
                <div  id="dialog-custom-style">
                    <SlideBar :images="imageLink"/>
                    <div class="field-center">
                        <button class="btn-theme btn-red no-border" type="submit">Masuk</button>
                        <button class="btn-theme btn-white no-border" type="submit" >Daftar</button> 
                    </div>
                </div>
            </template>
        </DialogComponent> 

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
            DialogComponent: () => import('@/components/Dialog/DialogComponent'),
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
        data() {
            return {
                 isModalVisible: false,
                 image: require("@/static/images/logo/people-icon.png"),
                 imageLink: [
                    {
                        id: 1, 
                        src: require('../static/images/slide-bar-image/image-1.jpg')
                    },
                    {
                        id: 2,
                        src: require('../static/images/slide-bar-image/image-2.jpg')
                    },
                ],
            }
        },
        methods: {
            showModal() {
                this.isModalVisible = true;
            },
            closeModal() {
                this.isModalVisible = false;
            }
        }
    };
</script>




