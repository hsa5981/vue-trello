<template>
    <div id="app">
        <NavBar></NavBar>
        <router-view></router-view>
    </div>
</template>

<script>
import NavBar from './components/Nav.vue'
export default {
  name: 'app',
  components: {NavBar},
  data () {
    return {
    }
  }
}
</script>

<style>

</style>
