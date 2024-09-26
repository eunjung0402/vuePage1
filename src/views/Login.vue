<template>
  <v-form>
    <v-container>
      <v-row>
        <v-col cols="12" sm="6" md="4">
          <v-text-field dense label="Regular"></v-text-field>
        </v-col>

        <v-col cols="12" sm="6" md="4">
          <v-text-field label="Filled" filled dense></v-text-field>
        </v-col>

        <v-col cols="12" sm="6" md="4">
          <v-text-field
            label="Filled"
            placeholder="Dense & Rounded"
            filled
            rounded
            dense
          ></v-text-field>
        </v-col>

        <v-col cols="12" sm="6" md="4">
          <v-text-field label="Solo" solo dense></v-text-field>
        </v-col>

        <v-col cols="12" sm="6" md="4">
          <v-text-field label="Outlined" outlined dense></v-text-field>
        </v-col>

        <v-col cols="12" sm="6" md="4">
          <v-text-field
            label="Outlined"
            placeholder="Placeholder"
            outlined
            dense
          ></v-text-field>
        </v-col>
      </v-row>
      <v-btn class="mr-4" type="submit" :disabled="invalid" @click="submit">
        submit
      </v-btn>
      <v-btn>
        clear
      </v-btn>
    </v-container>
  </v-form>
</template>

<script>
export default {
  name: "LoginPage",
  methods: {
    submit() {
      this.$router.push({ name: "Agree" }).catch(() => {
        this.$router.go(0);
      });
    },
  },
};
</script>

<style scoped>
.login {
  height: 300px;
  margin: 200px;
}
</style>
