<template>
  <div class="container">
    <side-bar />
    <v-main>
      <router-view />
    </v-main>
  </div>
</template>

<script>
import SideBar from "./components/SideBar.vue";
export default {
  components: { SideBar },
  name: "App",

  data: () => ({
    //
  }),
};
</script>