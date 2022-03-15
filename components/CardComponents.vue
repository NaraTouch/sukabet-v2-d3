<template>
    <div>
        <div class="display-card" v-for="(baccaratGame, index) in baccaratGames" :key="index">
            <b-card
                :img-src="baccaratGame.image"
                img-alt=""
                img-top
                tag="article"
                style="max-width: 20rem;"
                class="mb-2"
            >
                <span v-if="isActive" class="btn-theme gd-red-black no-border border-raduis-18" href="#" >Go somewhere</span>
                <span v-else href="#" >Go somewhere</span>
            </b-card>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        baccaratGames: Array,
        isActive: Boolean,
    },
    data() {
        return {
        }
    },
}
</script>