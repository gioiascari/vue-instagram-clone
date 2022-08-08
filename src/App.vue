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
      </div>
      <!-- /Barra di ricerca -->
      <v-spacer></v-spacer>
      <!-- Crea un nuovo post -->
      <v-btn depressed color="#E7596F" class="text-none mr-5">
        <span class="mr-2">
          <v-icon class="mr-2">mdi-plus</v-icon>Create New Post
        </span>
      </v-btn>
      <!-- /Crea un nuovo post -->
      <!-- Icons -->
      <v-btn icon class="mr-2">
        <v-icon>mdi-email-outline</v-icon>
      </v-btn>
      <v-btn icon class="mr-2">
        <v-icon>mdi-heart-outline</v-icon>
      </v-btn>
      <!-- /Icons -->
      <!-- Avatar -->
      <v-avatar size="40">
        <img lazy-src="img/me.jpg" src="img/me.jpg" alt="Gioia" />
      </v-avatar>
      <v-icon>mdi-menu-down</v-icon>
      <!--/ Avatar -->
    </v-app-bar>
    <main-nav />
    <v-content>
      <MainNav />
      <ProfileRightNav />
    </v-content>
  </v-app>
</template>

<script>
import ProfileRightNav from "./components/ProfileRightNav";
import MainNav from "./components/MainNav";

export default {
  name: "App",

  components: {
    MainNav,
    ProfileRightNav,
  },

  data: () => ({
    drawer: true,
    group: null,
  }),
  watch: {
    group() {
      this.drawer = false;
    },
  },
};
</script>
