<template>
<TopNavVue />
  <router-view/>
<MainFooter />
</template>

<script>
import TopNavVue from "./components/TopNav.vue";
import MainFooter from "./components/MainFooter.vue";

export default{
  components: {
    TopNavVue,
    MainFooter
}

}
</script>
<style>
#app {
  font-family: 'Roboto', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
