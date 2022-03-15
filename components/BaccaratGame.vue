<template>
    <div>
         <div id="baccarat-game" class="margin-space">
            <cardComponents :baccaratGames="gameLink" :isActive="isActive"  />
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
        }
    },
    
}
</script>