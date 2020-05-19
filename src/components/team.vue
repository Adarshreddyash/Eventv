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
            <span style="color: #4527A0;">Team&nbsp;</span>
          </b>
        </p>
        <p
          class="mt-3"
        >Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
          </v-flex>

        <v-flex xs6 sm3 md2 lg2 mx-sm-5 class="text-xs-center" style="text-align:center" v-for="k in team"  v-bind:key="k">
                   
                   <div 
                    class="text-xs-center ma-1 pa-1 py-5 my-0" >
                    <v-avatar size="100">
                        <v-img
                        :src="k.src"
                      :lazy-src="k.src">

                            <v-layout
                                slot="placeholder"
                                fill-height
                                align-center
                                justify-center
                                ma-0
                            >
                                <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
                            </v-layout>
                        
                        </v-img>
                    </v-avatar>
                    <p class="mt-3 mb-0 google-font" style="font-size:130%">{{k.name}}</p>
                   <p>Designation</p>
                   <v-btn class="mt-0 mx-0" icon :href="k.github" target="_blank">
                        <v-icon small style="color:#333">mdi-github</v-icon>
                    </v-btn>

                    <v-btn class="mt-0 mx-0" icon :href="k.linkedin" target="_blank">
                        <v-icon small style="color:#0077b5">mdi-linkedin</v-icon>
                    </v-btn>

                    <v-btn class="mt-0 mx-0" icon :href="k.twitter" target="_blank">
                        <v-icon small style="color:#0077b5">mdi-twitter</v-icon>
                    </v-btn>
                   </div>
                <br />
        </v-flex>

        
      </v-layout>
    </v-lazy>
  </v-container>
</template>

<script>
export default {
  name: "team",

  data: () => ({
      team: [
      { name: 'Member1',src:require('../assets/white_hoodie.png'),twitter:'https://twitter.com/adarshreddyash',github:'https://github.com/adarshreddyash',linkedin:'https://github.com/adarshreddyash'},
      { name: 'Member2',src:require('../assets/white_hoodie.png'),twitter:'https://twitter.com/adarshreddyash',github:'https://github.com/adarshreddyash',linkedin:'https://github.com/adarshreddyash'},
      { name: 'Member3',src:require('../assets/white_hoodie.png'),twitter:'https://twitter.com/adarshreddyash',github:'https://github.com/adarshreddyash',linkedin:'https://github.com/adarshreddyash'}
    ]
  })
};
</script>