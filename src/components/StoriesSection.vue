<template>
  <div>
    <v-layout>
      <v-flex>
        <div class="title">Featured Stories</div>
      </v-flex>
      <v-flex text-right>
        <v-btn depressed class="text-none" color="grey lighten-4">
          <span class="grey--text"> Popular Stories </span>
        </v-btn>
      </v-flex>
    </v-layout>
    <v-layout justify-start text-center class="mt-7">
      <!-- Image 1 -->
      <v-flex v-for="(account, i) in storiesAccount" :key="i">
        <v-avatar class="outlined" size="80">
          <v-avatar width="100%" height="100">
            <img :src="account.img" size="80" />
          </v-avatar>
        </v-avatar>
        <div class="subtitle-2">{{ account.name }}</div>
        <!--Card-->
      </v-flex>

      <!-- /Image 1 -->
    </v-layout>
  </div>
</template>

<script>
export default {
  name: "StoriesSection",
  data() {
    return {
      storiesAccount: [
        {
          name: "pablo",
          img: "https://images.unsplash.com/photo-1539571696357-5a69c17a67c6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80",
        },
        {
          name: "ghost.u",
          img: "https://images.unsplash.com/photo-1507038732509-8b1a9623223a?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80",
        },
        {
          name: "aioig",
          img: "https://images.unsplash.com/photo-1571914001156-dca4c3a20844?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=464&q=80",
        },
        {
          name: "iracsa",
          img: "https://images.unsplash.com/photo-1508002366005-75a695ee2d17?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=368&q=80",
        },
        {
          name: "badaboom",
          img: "https://images.unsplash.com/photo-1519689373023-dd07c7988603?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80",
        },
        {
          name: "default-name",
          img: "https://images.unsplash.com/photo-1558920558-feb6e762d597?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80",
        },
        {
          name: "bye-bye",
          img: "https://images.unsplash.com/photo-1613467678197-6054e47c5fc0?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=327&q=80",
        },
        {
          name: "pippo",
          img: "https://images.unsplash.com/photo-1615268485840-1616aebe9898?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=383&q=80",
        },
      ],
    };
  },
};
</script>

<style></style>
