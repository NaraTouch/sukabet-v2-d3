<template>
    <div id="slots-game">
        <div class="mb-2 mb-2-bgc">
            <div class="tabs box-shadow-1 bg-white gd-white-old">
                <div class="new-hot-offer">
                    <div></div>
                </div>
                <div class="row mr-0 ml-0">
                    <div class="col-3 pr-0 pl-0">
                        <li>
                            <a v-on:click="activetab=1" v-bind:class="[ activetab === 1 ? 'active' : '' ]">LAST WINNER</a>
                        </li>
                    </div>
                    <div class="col-3 pr-0 pl-0 r-l-border">
                        <li>
                            <a v-on:click="activetab=2" v-bind:class="[ activetab === 2 ? 'active' : '' ]">TOP WINNER</a>
                        </li>
                    </div> 
                   
                    <!-- <div class="col-3 pr-0 pl-0 r-l-border new-badge"> -->
                    <div class="col-3 pr-0 pl-0 r-l-border">
                        <li>
                            <a v-on:click="activetab=3" v-bind:class="[ activetab === 3 ? 'active' : '' ]">DAILY WIN</a>
                        </li>
                    </div>
                    <div class="col-3 pr-0 pl-0">
                        <li>
                            <a v-on:click="activetab=4" v-bind:class="[ activetab === 4 ? 'active' : '' ]">DAILY WIN</a>
                        </li>
                    </div>
                </div>
            </div>
            <div id="baccarat-game" class="col-lg-12  margin-space">
                <cardComponents :column-card="columnCard" :baccaratGames="baccaratGames" :isActive="isActive" />
            </div>
        </div>
    </div>
</template>

<script>
export default {
    components: {
        cardComponents: () => import('@/components/CardComponents'),
    },
    data () {
        return {
            isActive: false,
            activetab: 2,
            columnCard: 'col-xl-2 col-lg-3 col-md-6 col-sm-6 display-card',
            baccaratGames: [
                { 
                    id: 1,
                     image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                    title: '888',
                },
                {
                    id: 2,
                     image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 3,
                     image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 4,
                     image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 5,
                     image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 6,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                 { 
                    id: 1,
                     image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 2,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 3,
                     image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 4,
                     image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 5,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 6,
                     image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                 { 
                    id: 1,
                     image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 2,
                     image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 3,
                     image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 4,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 5,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 6,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                 { 
                    id: 1,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 2,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 3,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 4,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 5,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                },
                {
                    id: 6,
                    image: require('@/static/images/photos/poker-thumb.png'),
                    link: 'https://www.w3schools.com/',
                     title: '888',
                }
            ],
        }
    }
}
</script>