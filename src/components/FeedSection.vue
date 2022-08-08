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
    <v-row class="mt-5">
      <v-col>
        <v-card
          elevation="12"
          height="230"
          width="210"
          color="blue"
          class="mr-4"
        >
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
