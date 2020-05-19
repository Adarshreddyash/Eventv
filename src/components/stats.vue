<template>
 <v-container fluid class="pa-0">
        <v-layout wrap align-center justify-center row fill-height >
          <v-flex xs12 sm5 md8 lg8 xl8 class="pa-5">
        <p class="google-font mb-1" style="font-weight: 350;color: #616161;font-size:200%">
          <b>
            Wrap up with talks like
            <span style="color: #4527A0;">Docker , Kubernetes &nbsp;</span>and
            <span style="color: #4527A0;">Story Telling</span>
          </b>
        </p>
        <p
          class="mt-3"
        >Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
          </v-flex>
     
           <v-flex xs12 sm5 md6 lg5 xl6 class="pa-5">
        <v-layout row wrap class="px-5">
          <v-flex xs6 lg6>
            <p class="google-font mb-0" style="font-weight: 350;color: #616161;font-size:300%">
              <b>
                <v-icon size="80">mdi-code-tags</v-icon>
              </b>
            </p>
            <p>Codelabs</p>
          </v-flex>

          <v-flex xs6 lg6>
            <p class="google-font mb-0" style="font-weight: 350;color: #616161;font-size:300%">
              <b>
                 <v-icon size="80">mdi-account-group</v-icon>
              </b>
            </p>
            <p class="google-font">Collaborate</p>
          </v-flex>
          <v-flex xs6 lg6>
            <p class="google-font mb-0" style="font-weight: 350;color: #616161;font-size:300%">
              <b>
                <v-icon size="80">mdi-certificate-outline</v-icon>
              </b>
            </p>
            <p class="google-font">Certificate</p>
          </v-flex>
          <v-flex xs6 lg6>
            <p class="google-font mb-0" style="font-weight: 350;color: #616161;font-size:300%">
              <b>
              <v-icon size="80">mdi-tshirt-v-outline</v-icon>
              </b>
            </p>
            <p class="google-font">Goodies</p>
          </v-flex>
          
        </v-layout>
      </v-flex>
          <v-flex xs12 sm5 md6 lg3 xl6 class="pa-5">
        <v-layout row wrap class="px-5">
          <v-flex xs6 lg6>
            <p class="google-font mb-0" style="font-weight: 350;color: #616161;font-size:300%">
              <b>
                <span style="color: #4527A0;" >600+</span>
              </b>
            </p>
            <p class="google-font">Attendees</p>
          </v-flex>

          <v-flex xs6 lg6>
            <p class="google-font mb-0" style="font-weight: 350;color: #616161;font-size:300%">
              <b>
                <span style="color: #4527A0;">8+</span>
              </b>
            </p>
            <p class="google-font">Workshops</p>
          </v-flex>
          <v-flex xs6 lg6>
            <p class="google-font mb-0" style="font-weight: 350;color: #616161;font-size:300%">
              <b>
                <span style="color: #4527A0;">10+</span>
              </b>
            </p>
            <p class="google-font">Sessions</p>
          </v-flex>
          <v-flex xs6 lg6>
            <p class="google-font mb-0" style="font-weight: 350;color: #616161;font-size:300%">
              <b>
                <span style="color: #4527A0;">6+</span>
              </b>
            </p>
            <p class="google-font">Speakers</p>
          </v-flex>
          
        </v-layout>
      </v-flex>
        </v-layout>

    </v-container>
</template>

<script>
  export default {
    name: 'stats',

    data: () => ({
      
    }),
  }
</script>
<style scoped>
.pad-r8{
  padding-right: 70px;
}
</style>