<template>
  <div id="app">
    <Header></Header>
    <router-view>
      <Home></Home>
    </router-view>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Home from "@/views/Home.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "App",
  components: {
    Home,
    Footer,
    Header,
  },
};
</script>

<style scoped></style>
