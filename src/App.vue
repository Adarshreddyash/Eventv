<template>
  <v-app>
    <v-app-bar
      app
      color="white"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Eventv"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Eventv"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>
 
      <v-progress-linear
        indeterminate size="64"
        absolute
        bottom
        color="deep-purple accent-4"
        v-show="isLoading"
      ></v-progress-linear>

  
      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-content>
      <portfolio/>
    </v-content>
  </v-app>
</template>

<script>
import portfolio from './components/portfolio';

export default {
  name: 'App',

  components: {
    portfolio,
  },

  data: () => ({
    //
    isLoading: true,
  }),
 mounted() {
  setTimeout(() => {
    this.isLoading = false;
  }, 3000); // toggle after 5 seconds
}
};
</script>
