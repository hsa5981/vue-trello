<template>
    <div
        >Board
        <div>
            bid: {{bid}}
        </div>
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
