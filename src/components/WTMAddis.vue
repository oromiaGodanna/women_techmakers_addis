<template>
  <v-container class="px-10 py-10" style="background-color: white;">
    <v-layout wrap align-center justify-center row fill-height class="my-3">
      <v-flex xs12 md12 lg12 class="pa-2">
        <p class="google-font" style="font-size:120%">About {{chapterDetails.ChapterName}}</p>
        <p class="google-font" style="font-size:110%">{{chapterDetails.ChapterLongDec}}</p>
        <v-btn
          :href="chapterDetails.ChapterMeetupLink"
          target="_blank"
          outlined
          color="black"
          class="ma-0 google-font"
          style="border-radius:5px;text-transform: capitalize;"
        >Meetup Page</v-btn>&nbsp;
        <v-btn
          :href="chapterDetails.socialLinks[0].link"
          target="_blank"
          outlined
          color="black"
          class="ma-0 google-font"
          style="border-radius:5px;text-transform: capitalize;"
        >Facebook Page</v-btn>&nbsp;
        <v-btn
          :href="chapterDetails.socialLinks[3].link"
          target="_blank"
          outlined
          color="black"
          class="ma-0 google-font"
          style="border-radius:5px;text-transform: capitalize;"
        >Telegram Channel</v-btn>&nbsp;
        <v-btn
          :href="chapterDetails.socialLinks[1].link"
          target="_blank"
          outlined
          color="black"
          class="ma-0 google-font"
          style="border-radius:5px;text-transform: capitalize;"
        >Twitter Page</v-btn>
        <br />
        <br />
        <router-link
          to="/about"
          class="google-font"
          style="text-decoration:none;color:black"
        >See More about {{chapterDetails.ChapterName}}</router-link>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import ChapterDetails from "@/assets/data/chapterDetails.json";
export default {
  data() {
    return {
      chapterDetails: ChapterDetails
    };
  }
};
</script>