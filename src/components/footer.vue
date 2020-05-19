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
        <v-layout wrap align-center justify-center row fill-height >
           <v-flex xs12 sm5 md3 lg3 xl3 class="text-xs-center" style="margin:30px">
                <v-img
                    src="../assets/22.png"
                    width="100%">
                    <v-layout
                        slot="placeholder"
                        fill-height
                        align-center 
                        justify-center
                        ma-0
                    >
                    </v-layout>
                </v-img>
            </v-flex> 
            <v-flex xs11 sm8 md8 lg8 xl8 mx-sm-5>
                <p class="mb-1" style="font-weight: 350;color: #616161;font-size:300%"><b>Join us for digital
                    <span style="color: #4527A0;">well-being</span>.</b>
                </p>
                <p class="mt-0" style="font-size:180%">Eventv Event</p>
                <p class="" style="font-size:110%">Eventv is an event that focuses on collecting interested developers all over to tackle with the worlds
                  problems and solve them with the advanced technologies in the world. </p>
                <p class="" style="">
                  <v-chip
                      class="ma-2"
                       text-color="white"
                        >
               <v-avatar left><v-icon>mdi-calendar-month-outline</v-icon>
                 </v-avatar>
                <span style="color:#000000;"> November 23, 2020 </span>
                 </v-chip>

                 <v-chip
                      class="ma-2"
                       text-color="white"
                        >
               <v-avatar left><v-icon>mdi-map-marker</v-icon>
                 </v-avatar>
                <span style="color:#000000;">Warangal</span>
                 </v-chip>
                </p>

                <v-btn href="#" target="_blank" class="ma-0 elevation-1" color="#4527A0" style="text-transform: capitalize;border-radius:5px;color:white">Attend Event</v-btn>

                &nbsp;

                <v-btn href="#" target="_blank" rounded color="cyan" style="text-transform: capitalize;border-radius:5px;text-transform: capitalize;" outlined  class="ml-0" dark>Contact Us</v-btn>

            </v-flex>
        </v-layout>
 </v-lazy>
    </v-container>
</template>

<script>
  export default {
    name: 'footer',
    
    data: () => ({
      
    }),
  }
</script>
