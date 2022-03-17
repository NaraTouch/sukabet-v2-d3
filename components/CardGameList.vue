<template>
    <div id="row-card">
        <b-card no-body class="overflow-hidden card-size col-lg-6 col-md-6 col-sm-6 col-xs-12" v-for="(card, index) in cards" :key="index" >
            <div class="card-space">
            <b-row no-gutters class="border-card-style box-shadow-1">
            <b-col >
                <b-card-img :src="card.src" alt="Image" class="rounded-0"></b-card-img>
            </b-col>
            <b-col >
                <b-card-body :title="card.header">
                <b-card-text>
                    {{card.content}}
                </b-card-text>
                    <div class="input-group mr-sm-2 d-block button-style">
                        <button :href="card.link" type="submit" class="btn-size btn-theme gd-red-black no-border border-raduis-18">Main</button>
                    </div>
                </b-card-body>
            </b-col>
            </b-row>
            </div>
        </b-card>
    </div>
</template>

<script>
export default {
    data() {
        return {
            cards: [
                    {
                        header: 'Baccarat',
                        src: require('../static/images/photos/poker-thumb.png'),
                        content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere voluptatibus aliquam reprehenderit fugit iste',
                        link: 'https://www.w3schools.com/',
                    },
                    {
                        header: 'Sports',
                        src: require('../static/images/photos/poker-thumb.png'),
                        content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere voluptatibus aliquam reprehenderit fugit iste',
                        link: 'https://www.w3schools.com/',
                    },
                    {
                        header: 'Casino',
                        src: require('../static/images/photos/poker-thumb.png'),
                        content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere voluptatibus aliquam reprehenderit fugit iste',
                        link: 'https://www.w3schools.com/',
                    },
                    {
                        header: 'SLots',
                        src: require('../static/images/photos/poker-thumb.png'),
                        content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere voluptatibus aliquam reprehenderit fugit iste',
                        link: 'https://www.w3schools.com/',
                    },
                      {
                        header: 'Togel',
                        src: require('../static/images/photos/poker-thumb.png'),
                        content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere voluptatibus aliquam reprehenderit fugit iste',
                        link: 'https://www.w3schools.com/',
                    },
                    {
                        header: 'Arcade',
                        src: require('../static/images/photos/poker-thumb.png'),
                        content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere voluptatibus aliquam reprehenderit fugit iste',
                        link: 'https://www.w3schools.com/',
                    },
                ]
        }
    },
}
</script>



