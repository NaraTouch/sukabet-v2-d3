<template>
    <div class="mb-2">
        <div class="tabs">
            <div class="row mr-0 ml-0">
                <div class="col-4 pr-0 pl-0">
                    <li>
                        <a v-on:click="activetab=1" v-bind:class="[ activetab === 1 ? 'active' : '' ]">LAST WINNER</a>
                    </li>
                </div>
                <div class="col-4 pr-0 pl-0 r-l-border">
                    <li>
                        <a v-on:click="activetab=2" v-bind:class="[ activetab === 2 ? 'active' : '' ]">TOP WINNER</a>
                    </li>
                </div>
                <div class="col-4 pr-0 pl-0">
                    <li>
                        <a v-on:click="activetab=3" v-bind:class="[ activetab === 3 ? 'active' : '' ]">DAILY WIN</a>
                    </li>
                </div>
            </div>
        </div>
        <div class="content">
            <div v-if="activetab === 1" class="tabcontent">
                <LastWinner />
            </div>
            <div v-if="activetab === 2" class="tabcontent">
                <LastWinner />
            </div>
            <div v-if="activetab === 3" class="tabcontent">
                <LastWinner />
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        components: {
            LastWinner: () => import("@/components/LastWinner"),
        },
        data () {
            return {
                activetab: 1
            }
        }
    };
</script>
