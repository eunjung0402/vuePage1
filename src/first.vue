<template>
  <v-app id="inspire">
    <v-navigation-drawer v-model="drawer" app>
      <!--  -->
      <v-list>
        <v-list-item-group v-model="model" mandatory color="indigo">
          <v-list-item
            v-for="(item, i) in items"
            :key="i"
            @click="clickAction(item)"
          >
            <v-list-item-icon>
              <v-icon v-text="item.icon"></v-icon>
            </v-list-item-icon>

            <v-list-item-content>
              <v-list-item-title v-text="item.text"></v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer"> </v-app-bar-nav-icon>

      <v-toolbar-title>테스트</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <!--  -->
      <!-- <hello-world></hello-world> -->
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
// import HelloWorld from "@/components/HelloWorld.vue";

export default {
  data: () => ({
    drawer: null,
    items: [
      {
        icon: "mdi-wifi",
        text: "Wifi",
        pathName: "Test1",
        bb: "",
      },
      {
        icon: "mdi-bluetooth",
        text: "Bluetooth",
        pathName: "Test2",
      },
      {
        icon: "mdi-chart-donut",
        text: "Data Usage",
        pathName: "Test3",
      },
    ],
    model: 0,
  }),
  methods: {
    clickAction(item) {
      this.$router.push({ name: item.pathName }).catch(() => {
        this.$router.go(0);
      });
    },
  },
};
</script>
