<template>
  <div>
    <v-sheet color="#5708A6" dark>
      <v-container class="py-8 text-center">
        <div class="text-overline mb-3">Votility Protocol</div>
        <div class="text-h3">The simplest way to build your next DAO</div>

        <v-btn @click="goToBlog" large color="#dc591a" class="mt-4 w-full w-sm-auto">
          Get Started
          <v-icon right>mdi-menu-right</v-icon>
        </v-btn>
      </v-container>
    </v-sheet>
    <v-footer>
      <v-container>
        <div class="d-flex flex-column flex-md-row align-center justify-md-space-between">
          <div class="d-flex flex-column flex-md-row align-center">
           
          </div>
          <div>
            <v-btn @click="goToTrello()" icon color="secondary lighten-3" class="ml-2"><v-icon>mdi-trello</v-icon></v-btn>
            <v-btn @click="goToWhitepaper()" icon color="secondary lighten-3" class="ml-2"><v-icon>mdi-file-document-outline</v-icon></v-btn>
            <v-btn @click="goToTwitter()" icon color="secondary lighten-3" class="ml-2"><v-icon>mdi-twitter</v-icon></v-btn>
            <v-btn @click="goToGithub()" icon color="secondary lighten-3" class="ml-2"><v-icon>mdi-github</v-icon></v-btn>
            <v-btn icon color="secondary lighten-3" class="ml-2"><v-icon>mdi-discord</v-icon></v-btn>
          </div>
        </div>
        <v-divider class="my-3"></v-divider>
        <div class="d-flex flex-column flex-md-row align-center justify-md-space-between body-2">
          <div class="my-1 secondary--text">© Votility Protocol. All Rights Reserved</div>
        </div>
      </v-container>
    </v-footer>
  </div>
</template>

<script>
export default {
  methods: {
    goToWhitepaper() {
      window.location = '/whitepaper/whitepaper-v1.0.0.pdf';
    },

    goToBlog() {
      window.location = 'https://blog.votility.io';
    },

    goToTrello() {
      window.location = 'https://trello.com/votilityprotocol';
    },

    goToTwitter() {
      window.location = 'https://twitter.com/votilityp';
    },

    goToGithub() {
      window.location = 'https://github.com/votility';
    }
  }
}
</script>