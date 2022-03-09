<template>
    <section class="lastwinner-area lastwinner-default-area">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="lastwinner-content lastwinner-list lastwinner-list-scroll" data-aos="fade-up" data-aos-duration="1000">
                        <div class="lastwinner-item">
                            <div class="col-3 pr-0 pl-0">
                                <div class="thumb">
                                    <n-link to="/event-details">
                                        <img class="thumb-img" src="/images/events/50x50.jpg" alt="Image">
                                    </n-link>
                                </div>
                            </div>
                            <div class="col-9 pr-0 pl-0">
                                <div class="content">
                                    <h4 class="lastwinner-name">
                                        <n-link to="/event-details">WonderXXX   <span>just now</span></n-link>
                                    </h4>
                                    <div class="lastwinner-info"><span>2400K IDR  </span>in Poker</div>
                                </div>
                            </div>
                        </div>
                        <div class="lastwinner-item">
                            <div class="col-3 pr-0 pl-0">
                                <div class="thumb">
                                    <n-link to="/event-details">
                                        <img class="thumb-img" src="/images/events/50x50.jpg" alt="Image">
                                    </n-link>
                                </div>
                            </div>
                            <div class="col-9 pr-0 pl-0">
                                <div class="content">
                                    <h4 class="lastwinner-name">
                                        <n-link to="/event-details">WonderXXX   <span>just now</span></n-link>
                                    </h4>
                                    <div class="lastwinner-info"><span>2400K IDR  </span>in Poker</div>
                                </div>
                            </div>
                        </div>
                        <div class="lastwinner-item">
                            <div class="col-3 pr-0 pl-0">
                                <div class="thumb">
                                    <n-link to="/event-details">
                                        <img class="thumb-img" src="/images/events/50x50.jpg" alt="Image">
                                    </n-link>
                                </div>
                            </div>
                            <div class="col-9 pr-0 pl-0">
                                <div class="content">
                                    <h4 class="lastwinner-name">
                                        <n-link to="/event-details">WonderXXX   <span>just now</span></n-link>
                                    </h4>
                                    <div class="lastwinner-info"><span>2400K IDR  </span>in Poker</div>
                                </div>
                            </div>
                        </div>
                        <div class="lastwinner-item">
                            <div class="col-3 pr-0 pl-0">
                                <div class="thumb">
                                    <n-link to="/event-details">
                                        <img class="thumb-img" src="/images/events/50x50.jpg" alt="Image">
                                    </n-link>
                                </div>
                            </div>
                            <div class="col-9 pr-0 pl-0">
                                <div class="content">
                                    <h4 class="lastwinner-name">
                                        <n-link to="/event-details">WonderXXX   <span>just now</span></n-link>
                                    </h4>
                                    <div class="lastwinner-info"><span>2400K IDR  </span>in Poker</div>
                                </div>
                            </div>
                        </div>
                        <div class="lastwinner-item">
                            <div class="col-3 pr-0 pl-0">
                                <div class="thumb">
                                    <n-link to="/event-details">
                                        <img class="thumb-img" src="/images/events/50x50.jpg" alt="Image">
                                    </n-link>
                                </div>
                            </div>
                            <div class="col-9 pr-0 pl-0">
                                <div class="content">
                                    <h4 class="lastwinner-name">
                                        <n-link to="/event-details">WonderXXX   <span>just now</span></n-link>
                                    </h4>
                                    <div class="lastwinner-info"><span>2400K IDR  </span>in Poker</div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    import CoolLightBox from 'vue-cool-lightbox'
    import 'vue-cool-lightbox/dist/vue-cool-lightbox.min.css'

    export default {
        components: {
            CoolLightBox,
        },

        data() {
            return {
                items: [
                    {
                        src: "https://www.youtube.com/watch?v=eS9Qm4AOOBY",
                        autoplay: true
                    },
                ],
                index: null
            }
        },
    };
</script>