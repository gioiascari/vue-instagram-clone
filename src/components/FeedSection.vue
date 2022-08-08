<template>
  <div class="mt-10">
    <v-layout>
      <!-- Title -->
      <v-flex>
        <div class="title">Latest Feed</div>
      </v-flex>
      <!-- /Title -->
      <!-- Icons -->
      <v-flex text-right>
        <!-- Menù -->
        <v-btn icon>
          <v-icon>mdi-menu</v-icon>
        </v-btn>
        <!-- Menù -->
        <v-btn color="#E7596F">
          <v-icon>mdi-view-grid-outline</v-icon>
        </v-btn>
        <!-- /Menù -->
      </v-flex>
      <!-- /Icons -->
    </v-layout>

    <v-row class="mt-5" text-left>
      <v-col v-for="(image, i) in feedImg" :key="i">
        <v-card height="230" width="210" class="mr-4 my-5" outlined>
          <div class="subtitle-2 pa-md-4">
            {{ image.name }}
          </div>
          <v-img height="230" :src="image.img"></v-img>
          <div class="subtitle-2 pa-md-4">ciao</div>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "FeedSection",
  data() {
    return {
      feedImg: [
        {
          name: "uiuxdesign.trends",
          img: "https://images.unsplash.com/photo-1502429892517-ebe1510442a4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80",
        },
        {
          name: "mattwmurray",
          img: "https://images.unsplash.com/photo-1483728642387-6c3bdd6c93e5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1055&q=80",
        },
        {
          name: "lauvdahl",
          img: "https://images.unsplash.com/photo-1584701782235-beff0661e16a?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=675&q=80",
        },
        {
          name: "southpark",
          img: "https://images.unsplash.com/photo-1492056128351-09fb7a99969e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=562&q=80",
        },
        {
          name: "beyonce",
          img: "https://images.unsplash.com/photo-1495954484750-af469f2f9be5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80",
        },
        {
          name: "wacom",
          img: "https://images.unsplash.com/photo-1515966097209-ec48f3216288?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80",
        },
      ],
    };
  },
};
</script>

<style></style>
