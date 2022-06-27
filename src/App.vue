<template>
  <v-app class="grey ligthen-4">
    <NaviTodo></NaviTodo>
    <v-content> </v-content>
  </v-app>
</template>

<script>
import NaviTodo from "./components/NavbarTodo.vue";
export default {
  name: "App",
  data: () => ({
    //
  }),
  components: { NaviTodo },
};
</script>
