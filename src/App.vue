<template>
  <v-app>
    <v-app-bar flat app clipped-right color="white" clipped>
      <div class="d-flex align-center">
        <!-- Barra di ricerca -->
        <v-card color="grey lighten-4" outlined width="300px" class="pa-2 ml-4">
          <v-layout>
            <v-flex>
              <v-icon color="grey">mdi-magnify</v-icon>
            </v-flex>
            <v-flex class="text-right">
              <v-icon color="grey">mdi-microphone-outline </v-icon>
            </v-flex>
          </v-layout>
        </v-card>
        <!-- /Barra di ricerca -->
        <v-spacer></v-spacer>
        <!-- Crea un nuovo post -->
        <v-btn depressed color="#E7596F" class="text-none mr-5">
          <span class="mr-2">
            <v-icon class="mr-2">mdi-plus</v-icon>Create New Post
          </span>
        </v-btn>
        <!-- Icons -->
        <v-btn icon class="mr-2">
          <v-icon>mdi-email-outline</v-icon>
        </v-btn>
        <v-btn icon class="mr-2">
          <v-icon>mdi-heart-outline</v-icon>
        </v-btn>
        <!-- /Icons -->
        <v-avatar size="40">
          <img lazy-src="img/me.jpg" src="img/me.jpg" alt="Gioia" />
        </v-avatar>

        <!-- /Crea un nuovo post -->
      </div>

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

    <v-main>
      <HelloWorld />
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
