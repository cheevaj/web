<template>
  <div>
    <v-card style="height: 920px; background-color: #a0aecd">
      <v-col cols="12" class="pa-0" style="height: 20%">
        <v-row>
          <v-col cols=""> </v-col>
          <v-col> </v-col>
        </v-row>
        <v-img
          style="height: 100%; width: 100%"
          src="https://cdn.pixabay.com/photo/2017/06/06/22/46/mediterranean-cuisine-2378758_1280.jpg"
        />
      </v-col>
      <v-col cols="12" style="height: 80%">
        <v-row>
          <v-col cols="3" class="px-0">
            <pageowner_pc />
          </v-col>
          <v-col cols="6" class="px-1" style="height: 560px">
            <pagemenu_pc />
          </v-col>
          <v-col cols="3" class="px-0" style="height: 560px">
            <pagerestaurant_pc />
          </v-col>
        </v-row>
        <v-card-text style="height: 95px"> </v-card-text>
      </v-col>
    </v-card>
  </div>
</template>
  <script>
import pageowner_pc from "./pageowner_pc.vue";
import pagemenu_pc from "./pagemenu_pc.vue";
import pagerestaurant_pc from "./pagerestaurant_pc.vue";
export default {
  name: "IndexPage",
  components: {
    pageowner_pc,
    pagerestaurant_pc,
    pagemenu_pc,
  },
  data() {
    return {
      item: {},
    };
  },
};
</script>