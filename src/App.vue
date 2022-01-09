<template>
  <div id="app">
    <Header />
    <main>
      <DiscList />
      <DiscCard />
    </main>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import DiscList from "./components/DiscList.vue";
import DiscCard from "./components/DiscCard.vue";


export default {
  name: "App",
  components: {
    Header,
    DiscList,
    DiscCard
  },
};
</script>

<style lang="scss">
@import './style/general.scss';
</style>
