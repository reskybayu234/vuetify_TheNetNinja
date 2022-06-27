<template>
  <nav>
    <v-toolbar flat app>
      <v-toolbar-title class="text-uppercase grey--text">
        <v-btn
          class="btn1"
          @click="drawer = !drawer"
          fab
          small
          depressed
          color="grey"
        >
          <v-icon>mdi-circle-double</v-icon>
        </v-btn>
        <span class="font-weight-light">Todo</span>
        <span>Ninja</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn depressed>
        <span>Sign Out</span>
        <!-- <font-awesome-icon icon="fa-alicorn" /> -->
        <!-- <v-icon right>fas fa-right-from-bracket</v-icon> -->
        <v-icon right>mdi-logout</v-icon>
      </v-btn>
    </v-toolbar>

    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="mini"
      absolute
      dark
      temporary
    >
    </v-navigation-drawer>
  </nav>
</template>
<script>
export default {
  data() {
    return {
      drawer: true,
    };
  },
};
</script>

<style scoped>
.btn1 {
  min-width: 10px;
  height: 20px;
  width: 20px;
}
</style>