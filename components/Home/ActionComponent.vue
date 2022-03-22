<template>
    <div class="main-social">
        <a class="icon-image" target="_blank" href="#"><img :src="emoji"></a>
        <div class="offer icon-image">
            <a class="" target="_blank" href="#"><img :src="emoji"></a>
        </div>
        <a class="icon-image" target="_blank" href="#"><img :src="emoji"></a>
        <a class="icon-image" target="_blank" href="#"><img :src="emoji"></a>
    </div>
</template>

<script>
export default {
    data() {
        return {
            emoji: require("@/static/images/logo/people-icon.png"),
        }
    },
}
</script>
