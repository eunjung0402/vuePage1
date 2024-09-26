<template>
  <v-app id="inspire">
    <!-- <v-navigation-drawer v-model="drawer" app> </v-navigation-drawer> -->

    <v-app-bar app>
      <!-- <v-app-bar-nav-icon @click="drawer = !drawer"> </v-app-bar-nav-icon> -->
      <v-toolbar-title @click="home">PRIROS</v-toolbar-title>
      <ul>
        <li @click="loginPage">로그인</li>
        <li @click="helpPage">헬프센터</li>
      </ul>
    </v-app-bar>
  </v-app>
</template>

<script>
export default {
  name: "Header",
  data: () => ({ drawer: null }),
  methods: {
    loginPage() {
      this.$router.push({ name: "Login" }).catch(() => {
        this.$router.go(0);
      });
    },
    helpPage() {
      this.$router.push({ name: "Help" }).catch(() => {
        this.$router.go(0);
      });
    },
    home() {
      this.$router.push({ name: "Home" }).catch(() => {
        this.$router.go(0);
      });
    },
  },
};
</script>

<style scoped>
#inspire {
  height: 0;
  width: 100%;
}
</style>
