
<template>
<span>
   <v-navigation-drawer app v-model="drawer" class="brown lighten-2" dark disable-resize-watcher>
            <v-list>
                <template v-for="(item, index) in items">
                    <v-list-title :key="index">
                        <v-list-tile-content>
                            {{item.title}}
                        </v-list-tile-content>
                    </v-list-title>
                    <v-divider :key="`divider-${index}`"></v-divider>
                </template>
            </v-list>
        </v-navigation-drawer>
  <v-app-bar app flat class="ml-0 google-font" color="transparent" style="color: white;">
    <v-toolbar-side-icon class="hidden-md-and-up"  @click="drawer = !drawer"></v-toolbar-side-icon>
    <v-spacer class="hidden-md-and-up"></v-spacer>
    <v-toolbar-title>
      <v-avatar :title="true">
        <v-img src="../../src/assets/favicon-196x196.png" alt contain height="70%" width="70%"></v-img>
      </v-avatar>
      <span flat>{{title}}</span>
    </v-toolbar-title>

    <v-spacer></v-spacer>

    <v-toolbar-items>
      <v-btn style="color: white;" text>Home</v-btn>
      <v-btn text style="color: white;">About</v-btn>
      <v-btn text style="color: white;">Events</v-btn>
      <v-btn text style="color: white;">Team</v-btn>
      <v-btn text style="color: white;">Contact</v-btn>
    </v-toolbar-items>

    <!-- <template v-if="$vuetify.breakpoint.smAndUp">
        <v-btn icon>
          <v-icon>twitter</v-icon>
        </v-btn>
        <v-btn icon>
          <v-icon>facebook</v-icon>
        </v-btn>
        <v-btn icon>
          <v-icon>telegram</v-icon>
        </v-btn>
    </template>-->
  </v-app-bar>
  <!-- </div> -->

  <!-- <nav class="google-font">
        <v-app-bar flat app class="pl-6">
            <v-toolbar-title  class="ml-0 google-font  "
      style="text-transform: capitalize; color=transparent;" >
                Women Techmakers Addis
            </v-toolbar-title>
            <v-spacer></v-spacer>
            <v-toolbar-items  >
                <v-btn text class="ml-0 google-font  "
      style="text-transform: capitalize; color:#3f3f3f;">
                    Home
                </v-btn>
                <v-btn text class="ml-0 google-font  "
      style="text-transform: capitalize; color:#3f3f3f;">
                    About
                </v-btn>
                <v-btn text class="ml-0 google-font  "
      style="text-transform: capitalize; color:#3f3f3f;">
                    Events
                </v-btn>
                <v-btn text class="ml-0 google-font  "
      style="text-transform: capitalize; color:#3f3f3f;">
                    Team
                </v-btn>
                <v-btn text class="ml-0 google-font  "
      style="text-transform: capitalize; color:#3f3f3f;">
                    Contact
                </v-btn>

            </v-toolbar-items>

        </v-app-bar>
  </nav>-->
</span>
</template>


<script>
//based on the the content you're at change the title color or visibility
//based on the content you're at change background color of toolbar
export default {
  name: "ToolBar",
  components: {},

  data(){
    return {
      title: 'Women Techmakers Addis',
      drawer: false,
      items: [
                { title: "Menu" },
                { title: "Sign In"},
                { title: "Join" }
            ]
        };
  }
};
</script>
<style scoped>
</style>