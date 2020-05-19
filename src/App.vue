<template>
  <v-app>
    <v-app-bar
      app
      color="transparent"
      collapse-on-scroll
    >
      <div class="d-flex align-center">
       <v-toolbar-title color="secondary" style="font-weight:300px;font-size:35px;">Eventv</v-toolbar-title>
      </div>
 
      <v-progress-linear
        indeterminate size="64"
        absolute
        bottom
        color="deep-purple accent-4"
        v-show="isLoading"
      ></v-progress-linear>

  
      <v-spacer></v-spacer>

       <v-btn @click="switchTheme" icon>
        <v-icon>{{sicon}}</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-bell</v-icon>
      </v-btn>
      
    </v-app-bar>

    <v-content>
      <portfolio/>
    </v-content>
   
    <v-content>
      <stats/>
    </v-content>
     
     <v-content>
      <events/>
    </v-content>

    <v-content>
      <team/>
    </v-content>

    <v-content>
      <foo/>
    </v-content>


  </v-app>
</template>

<script>
import portfolio from './components/portfolio';
import stats from './components/stats';
import events from './components/events';
import team from './components/team';
import foo from './components/foo'
export default {
  name: 'App',
  inject: ['theme'],
  

  components: {
    portfolio,
    stats,
    events,
    team,
    foo,
  },

  data: () => ({
    //
    isLoading: true,
    sicon:'mdi-theme-light-dark',
  }),
  methods: {
    switchTheme() {
      const switchOff = this.$vuetify.dark ? 'theme--dark' : 'theme--light'
        , switchOn = this.$vuetify.dark ? 'theme--light' : 'theme--dark'
        , themed = document.getElementsByClassName( switchOff )

      Array.from(themed).forEach( (el) => {
        el.classList.remove( switchOff )
        el.classList.add( switchOn )
      })

      this.$vuetify.dark = ! this.$vuetify.dark
      this.theme.isDark = ! this.theme.isDark
    }
  },
 mounted() {
  setTimeout(() => {
    this.isLoading = false;
  }, 3000); // toggle after 3 seconds
}
};
</script>
