<template>
  <div>
    <v-card flat>
      <v-card height="40%">
        <v-card height="20%" class="rounded-0">
          <v-img
            style="padding-top: 1px; height: 100px;"
            class="pa-0"
            src="https://popmenucloud.com/usfzricy/4000d1c1-a311-4b56-806c-cb94773b3c51.jpg"
            />
          <!-- <div style="position: fixed; top: 65%; right: 10px">
        <v-btn fab color="primary" @click="newQuestion = !showDialog">
          <v-icon>mdi-plus</v-icon>
        </v-btn>
        </div> -->
        </v-card>
        <v-card class="rounded-0" height="100%">
          <!-- <v-card-text style="bottom: 100px;" class="text-h4 text-center" color="red">
        <h4>Restaurant</h4>
        </v-card-text> -->
          <v-col cols="12">
            <v-row>
              <v-col cols="3">
                <v-col class="py-0 text-center">
                  <v-icon size="25" color="#e0dc63">mdi-bowl-mix</v-icon>
                </v-col>
                <v-col class="py-0 text-center">ອາຫານ</v-col>
              </v-col>
              <v-col cols="3">
                <v-col class="py-0 text-center">
                  <v-icon size="25" color="#1abced"
                    >mdi-bottle-soda-classic</v-icon
                  >
                </v-col>
                <v-col class="py-0 text-center">ເຄື່ອງດື່ມ</v-col>
              </v-col>
              <v-col cols="3">
                <v-col class="py-0 text-center">
                  <v-icon size="25" color="#ababa7">mdi-pot-mix</v-icon>
                </v-col>
                <v-col class="py-0 text-center">ຕໍາ</v-col>
              </v-col>
              <v-col cols="3">
                <v-col class="py-0 text-center">
                  <v-icon size="25" color="#e0cc70">mdi-noodles</v-icon>
                </v-col>
                <v-col class="py-0 text-center">ອາຫານດ່ອນ</v-col>
              </v-col>
            </v-row>
          </v-col>
        </v-card>
      </v-card>
      <div class="pt-2">
        <foodpage_mb/>
      </div>
    </v-card>
  </div>
</template>
<script>
import foodpage_mb from './foodpage_mb.vue';
export default {
  name: "IndexPage",
    components: {
      foodpage_mb,
    },
    data() {
      return {
        
  
      };
    },
  data() {
    return {
      item: {},
    };
  },
  // mounted() {
  //   this.datas();
  // },
  // methods: {
  //   async datas() {
  //     const config ={
  //         headers: {
  //           'ngrok-skip-browser-warning': 'true', // Include the custom header
  //         },
  //       };
  //     const res = await this.$axios.$get(
  //       "https://220f-183-182-110-230.ngrok-free.app/users/object",config
  //     );
  //     console.log(res);
  //     this.item=res;
  //   },
  // },
};
</script>
