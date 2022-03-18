<template>
    <div class="row">
        <!-- <div class="col-xl-3 col-lg-4 col-md-6 col-sm-6 display-card" v-for="(baccaratGame, index) in baccaratGames" :key="index"> -->
        <div :class="columnCard" v-for="(baccaratGame, index) in baccaratGames" :key="index">
            <b-card
                :img-src="baccaratGame.image"
                img-alt=""
                img-top
                tag="article"
                style="max-width: 20rem;"
                class="mb-2"
            >
                <button v-if="isActive" type="buttom" class="btn-size btn-theme gd-red-black no-border border-raduis-18" href="#" >Main</button>
                <button v-else href="#" type="buttom">Main</button>
            </b-card>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        baccaratGames: Array,
        isActive: Boolean,
        columnCard: String,
    },
    data() {
        return {
        }
    },
}
</script>