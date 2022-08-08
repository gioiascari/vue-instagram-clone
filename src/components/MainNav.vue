<template>
  <v-navigation-drawer
    color="grey lighten-5"
    floating
    class="pa-4"
    app
    permanent
    v-model="drawer"
  >
    <!--Logo-->
    <v-layout class="pa-1">
      <div>
        <v-img
          width="130px"
          lazy-src="img/instagram_logo.svg.png"
          src="img/instagram_logo.svg.png"
          alt=""
        />
      </div>
    </v-layout>
    <!--/Logo-->

    <v-layout class="mt-10">
      <v-flex>
        <v-layout>
          <v-flex text-center>
            <!--Card-->
            <v-avatar class="outlined" size="80">
              <v-avatar size="70">
                <v-img
                  src="https://images.unsplash.com/photo-1554151228-14d9def656e4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=633&q=80"
                  lazy-src="https://images.unsplash.com/photo-1554151228-14d9def656e4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=633&q=80"
                />
              </v-avatar>
            </v-avatar>
            <!--Card-->
            <div class="mt-4 title">Eminem</div>
            <div class="mt-4 subtitle-2 grey--text">Los Angeles</div>
            <div class="mt-5">
              <v-layout>
                <v-flex>
                  <div class="subtitle-2">Post</div>
                  <div class="subtitle-2 grey--text">10</div>
                </v-flex>
                <v-flex>
                  <div class="subtitle-2">Followers</div>
                  <div class="subtitle-2 grey--text">50M</div>
                </v-flex>
                <v-flex>
                  <div class="subtitle-2">Following</div>
                  <div class="subtitle-2 grey--text">0</div>
                </v-flex>
              </v-layout>
            </div>
          </v-flex>
          <!--/Card-->
        </v-layout>
        <v-list nav dense class="mt-10">
          <v-list-item-group v-model="group" active-class="#E7596F--text">
            <!--Feed-->
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-home-outline</v-icon>
              </v-list-item-icon>
              <v-list-item-title>Feed</v-list-item-title>
            </v-list-item>
            <!--/Feed-->
            <!--Explore-->
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-compass-outline</v-icon>
              </v-list-item-icon>
              <v-list-item-title>Explore</v-list-item-title>
            </v-list-item>
            <!--/Explore-->
            <!--Trending-->
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-pound</v-icon>
              </v-list-item-icon>
              <v-list-item-title>Trending</v-list-item-title>
            </v-list-item>
            <!--/Trending-->
            <!--Top Post-->
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-check-decagram</v-icon>
              </v-list-item-icon>
              <v-list-item-title>Top Post</v-list-item-title>
            </v-list-item>
            <!--/Top Post-->
            <!--People-->
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-account-outline</v-icon>
              </v-list-item-icon>
              <v-list-item-title>People</v-list-item-title>
            </v-list-item>
            <!--/People-->
            <!--Notification-->
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-bell-outline</v-icon>
              </v-list-item-icon>
              <v-list-item-title>Notification</v-list-item-title>
            </v-list-item>
            <!--/Notification-->
            <!--Direct-->
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-send-outline</v-icon>
              </v-list-item-icon>
              <v-list-item-title>Direct</v-list-item-title>
            </v-list-item>
            <!--/Direct-->
            <!--Status-->
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-chart-pie</v-icon>
              </v-list-item-icon>
              <v-list-item-title>Status</v-list-item-title>
            </v-list-item>
            <!--/Status-->
            <!--Setting-->
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-cog-outline</v-icon>
              </v-list-item-icon>
              <v-list-item-title>Settings</v-list-item-title>
            </v-list-item>
            <!--/Setting-->
          </v-list-item-group>
        </v-list>
      </v-flex>
    </v-layout>
  </v-navigation-drawer>
</template>

<script>
export default {};
</script>

<style></style>
