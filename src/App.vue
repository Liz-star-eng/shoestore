<template>
<TopNavVue />
<MainContent />
<MainFooter />
  <router-view/>
</template>

<script>
import TopNavVue from "./components/TopNav.vue";
import MainContent from "./components/MainContent.vue";
import MainFooter from "./components/MainFooter.vue";

export default{
  components: {
    TopNavVue,
    MainContent,
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
