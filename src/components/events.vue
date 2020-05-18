<template>
  <v-container class="pa-0">
    <v-lazy
      v-model="isActive"
      :options="{
          threshold: .5
        }"
      min-height="200"
      transition="fade-transition"
    >
      <v-layout wrap align-center justify-center row fill-height>
          <v-flex xs12 sm12 md12 lg11 xl2 class="pa-5">
        <p class="mb-1" style="font-weight: 350;color: #616161;font-size:200%">
          <b>
            Our
            <span style="color: #4527A0;">Events&nbsp;</span>
          </b>
        </p>
        <p
          class="mt-3"
        >Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
          </v-flex>

        <v-flex xs12 sm3 md3 lg3 xl3 class="text-xs-center" style="margin:30px">
          <v-card class="mx-auto" max-width="344">
            <v-card-text>
              <div>1st Day</div>
              <p class="display-1 text--primary">Hands on with docker</p>
               <div class="text--primary">
                <v-chip class="mb-2" color="indigo" text-color="white">
                  <v-avatar left>
                    <v-img
                      class="elevation-6"
                      src="../assets/hat_man.png"
                    ></v-img>
                  </v-avatar>Sree Surya
                </v-chip>
                <br />
                <v-badge
                  color="deep-purple accent-4"
                  icon="mdi-amazon"
                  class="mt-5"
                  bordered
                  overlap
                >Design Engineer@</v-badge>
              </div>
            </v-card-text>
          </v-card>
        </v-flex>

        <v-flex xs11 sm3 md3 lg3 xl8 mx-sm-5 class="text-xs-center" style="margin:20px">
          <v-card class="mx-auto" max-width="344">
            <v-card-text>
              <div>2nd Day</div>
              <p class="display-1 text--primary">Hack on with Kubernetes</p>
              <div class="text--primary">
                <v-chip class="mb-2" color="indigo" text-color="white">
                  <v-avatar left>
                    <v-img
                      class="elevation-6"
                      size="30"
                      src="../assets/white_hoodie.png"
                    ></v-img>
                  </v-avatar>Adarshreddy Adelli
                </v-chip>
                <br />
                <v-badge
                  color="deep-purple accent-4"
                  icon="mdi-google"
                  class="mt-5"
                  bordered
                  overlap
                >Software Engineer @</v-badge>
              </div>
            </v-card-text>
          </v-card>
        </v-flex>

        <v-flex xs11 sm3 md3 lg3 xl8 mx-sm-5 class="text-xs-center" style="margin:20px">
          <v-card class="mx-auto" max-width="344">
            <v-card-text>
              <div>3rd Day</div>
              <p class="display-1 text--primary">Art of story telling</p>
             <div class="text--primary">
                <v-chip class="mb-2" color="indigo" text-color="white">
                  <v-avatar left>
                    <v-img
                      class="elevation-6"
                      size="30"
                      src="../assets/girl_smile.png"
                    ></v-img>
                  </v-avatar>Rishika Rao
                </v-chip>
                <br />
                <v-badge
                  color="deep-purple accent-4"
                  icon="mdi-apple"
                  class="mt-5"
                  bordered
                  overlap
                >Software Engineer @</v-badge>
              </div>
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-lazy>
  </v-container>
</template>

<script>
export default {
  name: "events",

  data: () => ({})
};
</script>