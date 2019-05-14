<template>
    <div
        >Board
        <div>
            bid: {{bid}}
        </div>
        <router-link :to="`/board/${bid}/card/1`">Card1</router-link>
        <router-link :to="`/board/${bid}/card/2`">Card2</router-link>
        <hr>
        <router-view></router-view>
    </div>
</template>

<script>
export default {
    data(){
        return {
            bid: 0
        }
    },
    created(){
        var params = this.$route.params
        this.bid = params.bid
    }
}
</script>

<style>

</style>
