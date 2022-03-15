<template>
    <div>
        <div class="mb-2 mb-2-bgc">
            <div class="tabs box-shadow-1 bg-white gd-white-old">
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
                    <div class="col-3 pr-0 pl-0 r-l-border new-badge">
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
            <div id="baccarat-game" class="margin-space game-center">
                <cardComponents :baccaratGames="baccaratGames" :isActive="isActive" />
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
            baccaratGames: [
                { 
                    id: 1,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 2,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 3,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 4,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 5,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 6,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                 { 
                    id: 1,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 2,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 3,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 4,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 5,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 6,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                 { 
                    id: 1,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 2,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 3,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 4,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 5,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 6,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                 { 
                    id: 1,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 2,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 3,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 4,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 5,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                },
                {
                    id: 6,
                    image: 'https://picsum.photos/600/300/?image=25',
                    link: 'https://www.w3schools.com/',
                }
            ],
        }
    }
}
</script>