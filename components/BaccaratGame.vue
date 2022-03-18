<template>
    <div class="row">
         <div id="baccarat-game" class="col-lg-12 margin-space">
            <cardComponents :column-card="columnCard" :baccaratGames="gameLink" :isActive="isActive"  />
        </div>
    </div>
</template>

<script>
export default {
    props: {
        gameLink: Array,
    },
    data() {
        return {
             components: {
                 cardComponents:() => import('@/components/CardComponents'),
             },
             isActive: true,
             columnCard: 'col-xl-3 col-lg-4 col-md-6 col-sm-6 display-card',
        }
    },
    
}
</script>