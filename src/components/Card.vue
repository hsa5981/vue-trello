<template>
    <div>
        Card
        <div>
            cid: {{cid}}
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return {
            cid: 0
        }
    },
    created(){
        var params = this.$route.params
        this.cid = params.cid
    },
    watch:{
        $route(){
            this.cid = this.$route.params.cid
        }
    }
}
</script>

<style>

</style>
