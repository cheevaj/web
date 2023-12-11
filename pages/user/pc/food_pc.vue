<template>
    <div>
      <v-row>
        <v-col cols="12" class="px-2">
          <v-card>
            <v-row class="px-3">
              <v-col cols="2">
                <v-img
                  src="https://womensfitness.co.uk/wp-content/uploads/sites/3/2022/11/Shutterstock_1675475479.jpg?w=900"
                />
              </v-col>
              <v-col cols="7">
                <v-card-title> ອາຫານລອມທອດ </v-card-title>
                <v-card-text>ລາຄາ: 120.000 kip </v-card-text>
              </v-col>
              <v-col cols="3" class="pt-6 pb-0">
                <v-row class="py-0">
                  <v-col cols="3" class="text-right pt-4"> ຈໍານວນ: </v-col>
                  <v-col cols="3" class="pt-2">
                    <v-text-field
                      class="pt-0"
                      label="1"
                      outlined
                      filled
                      dense
                    ></v-text-field>
                  </v-col>
                  <v-col cols="6">
                    <div class="pl-3">
                      <v-btn x-small class="px-0 py-4">
                        <v-icon size="30">mdi-chevron-left</v-icon>
                      </v-btn>
  
                      <v-btn x-small class="px-0 py-4 ml-2">
                        <v-icon size="30">mdi-chevron-right</v-icon>
                      </v-btn>
                    </div>
                  </v-col>
                </v-row>
                <v-col v-if="add" class=" pa-0 pb-4 text-center">
                  <v-btn
                    height="50"
                    width="150"
                    @click="Addmenu"
                    text
                    style="background-color: #00e32d; color: white"
                  >
                    <v-col>
                      <v-row>
                        <v-col cols="7" class="pt-4">
                          <h2>ສັ່ງ</h2>
                        </v-col>
                        <v-col cols="5">
                          <v-icon size="45">mdi-check-circle</v-icon>
                        </v-col>
                      </v-row>
                    </v-col>
                  </v-btn>
                </v-col>
                <v-col v-else class="pa-0 pb-4 text-center">
                  <v-btn
                    height="50"
                    width="150"
                    @click="add=true"
                    text
                    style="background-color: #ff4444; color: white"
                  >
                    <v-card-actions>
                      <div>
                        <h2>ຍົກເລີກ</h2>
                      </div>
                      <div>
                        <v-icon class="pl-2" size="45">mdi-close-octagon</v-icon>
                      </div>
                    </v-card-actions>
                  </v-btn>
                </v-col>
              </v-col>
            </v-row>
          </v-card>
        </v-col>
      </v-row>
    </div>
  </template>
  <script>
  export default {
    data() {
      return {
        add: true,
      };
    },
    methods: {
      Addmenu() {
        this.add = false;
      },
    },
  };
  </script>
  
  
  
  
  