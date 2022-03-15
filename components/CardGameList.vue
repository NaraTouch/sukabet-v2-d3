<template>
    <div id="row-card">
    <b-card no-body class="overflow-hidden" v-for="(card, index) in cards" :key="index" style="max-width: 580px;">
        <b-row no-gutters>
        <b-col md="6">
            <b-card-img :src="card.image" alt="Image" class="rounded-0"></b-card-img>
        </b-col>
        <b-col md="6">
            <b-card-body :title="card.header">
            <b-card-text>
                {{card.content}}
            </b-card-text>
                <div class="input-group mr-sm-2 d-block">
                    <button :href="card.link" type="submit" class="btn-theme gd-red-black no-border border-raduis-18">Main</button>
                </div>
            </b-card-body>
        </b-col>
        </b-row>
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
                        image: 'https://picsum.photos/400/400/?image=20',
                        content: ' This is a wider card with supporting text as a natural lead-in to additional content.This content is a little bit longer.',
                        link: 'https://www.w3schools.com/',
                    },
                    {
                        header: 'Baccarat',
                        image: 'https://picsum.photos/400/400/?image=20',
                        content: ' This is a wider card with supporting text as a natural lead-in to additional content.This content is a little bit longer.',
                        link: 'https://www.w3schools.com/',
                    },
                    {
                        header: 'Baccarat',
                        image: 'https://picsum.photos/400/400/?image=20',
                        content: ' This is a wider card with supporting text as a natural lead-in to additional content.This content is a little bit longer.',
                        link: 'https://www.w3schools.com/',
                    },
                    {
                        header: 'Baccarat',
                        image: 'https://picsum.photos/400/400/?image=20',
                        content: ' This is a wider card with supporting text as a natural lead-in to additional content.This content is a little bit longer.',
                        link: 'https://www.w3schools.com/',
                    },
                      {
                        header: 'Baccarat',
                        image: 'https://picsum.photos/400/400/?image=20',
                        content: ' This is a wider card with supporting text as a natural lead-in to additional content.This content is a little bit longer.',
                        link: 'https://www.w3schools.com/',
                    },
                    {
                        header: 'Baccarat',
                        image: 'https://picsum.photos/400/400/?image=20',
                        content: ' This is a wider card with supporting text as a natural lead-in to additional content.This content is a little bit longer.',
                        link: 'https://www.w3schools.com/',
                    },
                ]
        }
    },
}
</script>



