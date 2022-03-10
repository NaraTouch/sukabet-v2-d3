<template>
    <header class="header-area header-default p-0" :class="{'is-sticky': isSticky}">
        <div class="container pl-0 m-0 pr-0">
            <div class="row mr-0 ml-0 align-items-center justify-content-between">
                <div class="col-5 col-sm-3 col-lg-2 pr-0 pl-0 t-0">
                    <div class="header-logo-area">
                        <n-link to="/">
                            <img class="logo-main" src="/images/logo/logo.png" alt="Logo" />
                        </n-link>
                    </div>
                </div>
                <div class="col-7 col-sm-9 col-lg-10">
                    <div class="header-align">
                        <div class="header-navigation-area">
                            <LoginDesktop />
                        </div>
                        <div class="header-action-area">
                            <div class="mobile-menu-toggle d-lg-none">
                                <button class="toggle" @click="mobiletoggleClass('addClass', 'show-mobile-menu')">
                                    <i class="icon-top"></i>
                                    <i class="icon-middle"></i>
                                    <i class="icon-bottom"></i>
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="container pl-0 m-0 pr-0">
            <Navigation />
        </div>
    </header>
</template>

<script>
    export default {
        components: {
            Navigation: () => import("@/components/Navigation"),
            LoginDesktop: () => import("@/components/LoginDesktop"),
        },

        data() {
            return {
                isSticky: false,
            }
        },

        mounted(){
            window.addEventListener('scroll', () => {
                let scrollPos = window.scrollY
                if(scrollPos >= 200){
                    this.isSticky = true
                } else {
                    this.isSticky = false
                }
            })
        },

        methods: {
            // offcanvas mobile-menu
            mobiletoggleClass(addRemoveClass, className) {
                const el = document.querySelector('#offcanvas-menu');
                if (addRemoveClass === 'addClass') {
                    el.classList.add(className);
                } else {
                    el.classList.remove(className);
                }
            },
        },
    };
</script>