<template>
    <div>
      <div>
        <v-img
          style="height: 200px"
          src="https://st3.depositphotos.com/1037238/32919/v/1600/depositphotos_329191372-stock-illustration-chinese-restaurant-illustration.jpg"
        >
          <v-card-title style="color: #fff" class="text-h4 text--darken"
            >Chinese Restaurant Illustration
          </v-card-title>
        </v-img>
        <v-card-text class="text-h5">Chinese Restaurant Illustration</v-card-text>
      </div>
      <v-divider></v-divider>
      <div>
        <v-row>
          <v-col cols="4">
            <v-col cols="12" style="background-color: LightGray" class="pa-0">
              <v-card-text class="py-5">
                <h2>ໂຕະທີ່ 2</h2>
              </v-card-text>
            </v-col>
          </v-col>
          <v-col cols="8" class="pl-0">
            <v-col style="background-color: LightGray" cols="12" class="pl-0">
              <v-row>
                <v-col
                  cols="4"
                  class="my-auto py-3"
                  v-if="active1"
                  style="background-color: rgb(245, 245, 245)"
                >
                  <v-btn text>
                    <v-card-title class="py-2 my-0">
                      <div class="mx-auto">ປະເພດອາຫານ</div>
                    </v-card-title>
                  </v-btn>
                </v-col>
                <v-col cols="4" class="my-auto py-3" @click="onactive1" v-else>
                  <v-btn text>
                    <v-card-title class="py-2 my-0">
                      <div class="mx-auto">ປະເພດອາຫານ</div>
                    </v-card-title>
                  </v-btn>
                </v-col>
  
                <v-col
                  cols="4"
                  class="my-auto py-3"
                  v-if="active2"
                  style="background-color: rgb(245, 245, 245)"
                >
                  <v-btn text>
                    <v-card-title class="py-2 my-0">
                      <div class="mx-auto">ປະເພດຕໍາ</div>
                    </v-card-title>
                  </v-btn>
                </v-col>
                <v-col cols="4" class="my-auto py-3" @click="onactive2" v-else>
                  <v-btn text>
                    <v-card-title class="py-2 my-0">
                      <div class="mx-auto">ປະເພດຕໍາ</div>
                    </v-card-title>
                  </v-btn>
                </v-col>
  
                <v-col
                  cols="4"
                  class="my-auto py-3"
                  v-if="active3"
                  style="background-color: rgb(245, 245, 245)"
                >
                  <v-btn text>
                    <v-card-title class="py-2 my-0">
                      <div class="mx-auto">ປະເພດເຄື່ອງດື່ມ</div>
                    </v-card-title>
                  </v-btn>
                </v-col>
                <v-col cols="4" class="my-auto py-3" @click="onactive3" v-else>
                  <v-btn text>
                    <v-card-title class="py-2 my-0">
                      <div class="mx-auto">ປະເພດເຄື່ອງດື່ມ</div>
                    </v-card-title>
                  </v-btn>
                </v-col>
              </v-row>
            </v-col>
          </v-col>
        </v-row>
      </div>
      <v-divider></v-divider>
      <v-card-text class="pa-0 pt-2">
        <v-card-text class="scroll_y" style="height: 700px;">
          <food_pc />
        </v-card-text>
      </v-card-text>
      <div>
        <br />
        <v-divider></v-divider>
        <v-row class="px-4">
          <v-col cols="6" class="px-0">
            <v-card-text class="pt-0 px-0">
              <br />
              <v-card-title class="py-0"> ໃບບິນໂຕະ 2 </v-card-title>
              <v-divider></v-divider>
              <v-row>
                <v-col cols="6" class="text-center">ເມນູ</v-col>
                <v-col cols="6" class="text-center">ລາຄາ</v-col>
              </v-row>
              <v-card flat style="height: 350px; overflow-y: scroll">
                <v-col cols="12">
                  <v-divider></v-divider>
                  <v-card-text>
                    <v-row>
                      <v-col cols="6"> ff </v-col>
                      <v-col cols="6" class="text-right"> 50.000 kip</v-col>
                    </v-row>
                    <v-divider></v-divider>
                  </v-card-text>
                </v-col>
              </v-card>
              <v-divider></v-divider>
              <v-row>
                <v-col cols="7">
                  <v-card-actions>
                    <v-card-text class="py-2 pt-3">
                      <h3>ລາຄາໃບບີນລອມ:</h3>
                    </v-card-text>
                    <v-card-text class="py-2 pt-3 pl-0">50.000 kip</v-card-text>
                  </v-card-actions>
                </v-col>
                <v-col cols="5"> </v-col>
              </v-row>
            </v-card-text>
          </v-col>
          <v-col cols="6" class="px-0">
            <v-card-text class="pt-0 px-0">
              <br />
              <v-card-title class="py-0"> ສັ່ງເມນູໃໝ່ </v-card-title>
              <v-divider></v-divider>
              <v-row>
                <v-col cols="6" class="text-center">ເມນູ</v-col>
                <v-col cols="6" class="text-center">ລາຄາ</v-col>
              </v-row>
              <v-card flat style="height: 350px; overflow-y: scroll">
                <v-col cols="12">
                  <v-divider></v-divider>
                  <v-card-text >
                    <v-row>
                      <v-col cols="6"> ss </v-col>
                      <v-col cols="5" class="text-right"> 12.000 kip </v-col>
                      <v-col cols="1" class="pt-2 pa-0 text-right">
                        <v-icon size="30">mdi-close-octagon</v-icon>
                      </v-col>
                    </v-row>
                    <v-divider></v-divider>
                  </v-card-text>
                </v-col>
              </v-card>
              <v-divider></v-divider>
              <v-row>
                <v-col cols="7">
                  <v-card-actions >
                    <v-card-text class="py-2 pt-3">
                      <h3>ລາຄາສັ່ງລອມ:</h3>
                    </v-card-text>
                    <v-card-text class="py-2 pt-3 px-0 ">12.000 kip</v-card-text>
                  </v-card-actions>
                </v-col>
                <v-col cols="5">
                  <div class="py-2 pt-3">
                    <v-btn class="px-0 py-4"> ຢືນຢັນການສັ່ງ </v-btn>
                    <v-btn class="px-0 py-4 ml-3"> ຂໍຍົກເລີກ </v-btn>
                  </div>
                </v-col>
              </v-row>
            </v-card-text>
          </v-col>
        </v-row>
        
      </div>
    </div>
  </template>
  
  <script>
  import food_pc from "./food_pc.vue";
  export default {
    name: "IndexPage",
    components: {
      food_pc,
    },
    data() {
      return {
        active1: true,
        active2: false,
        active3: false,
        newQuestion:true,
  
      };
    },
    methods: {
      onactive1() {
        this.active1 = true;
        this.active2 = false;
        this.active3 = false;
      },
      onactive2() {
        this.active2 = true;
        this.active1 = false;
        this.active3 = false;
      },
      onactive3() {
        this.active3 = true;
        this.active1 = false;
        this.active2 = false;
      },
    },
  };
  </script>
  <style>
  .scroll_y {
    background-color: #eee;
    border: 1px dotted black;
    overflow-y: scroll; /* Add the ability to scroll */
  }
  
  /* Hide scrollbar for Chrome, Safari and Opera */
  .scroll_y::-webkit-scrollbar {
    display: none;
  }
  
  /* Hide scrollbar for IE, Edge and Firefox */
  .scroll_y {
    -ms-overflow-style: none; /* IE and Edge */
    scrollbar-width: none; /* Firefox */
  }
  </style>
  