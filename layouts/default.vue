<template>
  <div v-if="status === 'admin'">
    <div v-if="$vuetify.breakpoint.mobile">
      <v-app>
      </v-app>
    </div>
    <v-app v-else dark style="background-color: whitesmoke">
      <v-app-bar v-if="false" :clipped-left="clipped" fixed app>
        <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      </v-app-bar>
      <v-main>
        <home_on_pc />
      </v-main>
    </v-app>
  </div>
  <div v-else-if="status==='owner'">
    <div v-if="$vuetify.breakpoint.mobile">
      <v-app>
        <home_on_pc />
      </v-app>
    </div>
    <v-app v-else dark style="background-color: whitesmoke">
      <v-app-bar v-if="false" :clipped-left="clipped" fixed app>
        <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      </v-app-bar>
      <v-main>
        <home_on_pc />
      </v-main>
    </v-app>
  </div>
  <div v-else-if="status==='user'">
    <div v-if="$vuetify.breakpoint.mobile">
      <v-app>
        <home_mb />
      </v-app>
    </div>

    <v-app v-else dark style="background-color: whitesmoke">
      <v-app-bar v-if="false" :clipped-left="clipped" fixed app>
        <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      </v-app-bar>
      <v-main>
        <home_pc />
      </v-main>
    </v-app>
    
  </div>
  <div v-else>
    <v-app dark style="background-color: #74d3fc">
      <v-main>
        <Nuxt />
      </v-main>
    </v-app>
  </div>
</template>

<script>
import home_on_pc from "../pages/owner/home_on_pc.vue";
import food_mb from "../pages/food_mb.vue";
import home_mb from "../pages/user/mobile/home_mb.vue";
import home_pc from "../pages/user/pc/home_pc.vue";
export default {
  components: { food_mb, home_mb, home_pc,home_on_pc},
  name: "DefaultLayout",
  data() {
    return {
      status: "",
      icons: ["mdi-home", "mdi-email", "mdi-home", "mdi-delete", "mdi-home"],
      links: ["Home", "About Us", "Team", "Services", "Blog"],
      clipped: false,
      fixed: false,
      items: [
        {
          icon: "mdi-apps",
          title: "Welcome",
          to: "/",
        },
        {
          icon: "mdi-chart-bubble",
          title: "Inspire",
          to: "/inspire",
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: "Vuetify.js",
    };
  },
};
</script>


