<template>
  <v-navigation-drawer
    class="pa-4 mt-6"
    app
    clipped
    floating
    permanent
    right
    v-model="drawer"
  >
    <v-layout>
      <v-card height="300" width="100%">
        <v-img
          height="300"
          width="100%"
          src="https://images.unsplash.com/photo-1567304441104-d7a7d3e4bc1b?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=869&q=80"
        ></v-img>
      </v-card>
    </v-layout>
    <v-layout class="mt-6">
      <div class="title">Gioia Ascari</div>
    </v-layout>
    <v-layout>
      <v-flex>
        <v-layout>
          <div class="subtitle-2">400</div>
          <div class="subtitle-2 ml-1 grey--text">Photos</div>
        </v-layout>
      </v-flex>
      <v-flex>
        <v-layout>
          <div class="subtitle-2">527k</div>
          <div class="subtitle-2 ml-1 grey--text">Followers</div>
        </v-layout>
      </v-flex>
    </v-layout>
    <v-layout class="mt-3 subtitle-2 grey--text">
      I'm a full-stack developer based in Venice, Italy, always interested in
      learning about new Technologies and projects!
      <br />
      <br />
    </v-layout>
    <v-layout class="">
      <v-flex>
        <div class="subtitle-2">Locations</div>
        <div class="subtitle-2 grey--text">Based in Venice, Italy</div>
      </v-flex>
    </v-layout>
    <v-layout class="my-5">
      <v-flex>
        <div class="subtitle-2">Profession</div>
        <div class="subtitle-2 grey--text">Developer</div>
      </v-flex>
    </v-layout>
  </v-navigation-drawer>
</template>

<script>
export default {
  name: "ProfileRightNav",
};
</script>

<style></style>
