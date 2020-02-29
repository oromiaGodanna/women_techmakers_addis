<template>
<v-container class="px-10 py-10">
      <v-layout row wrap >  
        <v-flex xs12 sm4 md2 lg2 class="pa-4">
          <v-img
            :src="require('../assets/Images/svg/WTM-women.svg')"
            :lazy-src="require('../assets/Images/svg/WTM-women.svg')"
            width="100%"
          >
            <v-layout slot="placeholder" fill-height align-center justify-center ma-0>
              <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
            </v-layout>
          </v-img>
        </v-flex>
        <v-flex xs12 sm8 md10 lg10 class="pa-2 py-4 px-3">
          <p class="google-font mb-0" style="font-size:150%">Women Techmakers program</p>
          <p
            class="google-font mt-1"
            style="font-size:100%"
          >Google's Women Techmakers program provides visibility, community, and resources for women in technology. From 2014 to present, Women Techmakers is continually launching global scalable initiatives and piloting new programs to support and empower women in the industry.
                </p>
          <v-btn
          :href="ChapterDetails.wtmWebsite"
            target="_blank"
            outlined
            color="#4C4A78"
            class="ma-0 google-font"
            style="border-radius:7px;text-transform: capitalize;"
          >See More About WTM Program</v-btn>
        </v-flex>
      </v-layout>
    </v-container>
  <!-- <v-container class='spacing-playground px-6' >
      <v-layout row wrap justify-space-between>
          
          <v-flex class='spacing-playground px-6' xs11 sm11 md6 lg6>
              <p class="text-justify">
                
              </p>
              
            <v-btn
              href="www.womentechmakers.com"
              target="_blank"
              outlined
              text-color="#5BC7F8"
              class="ma-0 google-font"
              style="border-radius:7px;text-transform: capitalize;"
            >See More About WTM Program</v-btn>
          

          </v-flex>
          
          <v-flex xs11 sm11 md6 lg6>
              <youtube 
              :video-id="videoId" 
              :player-vars="playerVars" 
              @playing="playing"
               width="85%"
                height="170%">

              </youtube>
          </v-flex>
      </v-layout>
  </v-container> -->
</template>
<script>
import ChapterDetails from "@/assets/data/chapterDetails.json";
export default {
    data() {
    return {
        ChapterDetails: ChapterDetails,
      videoId: 'fknJH4qyOIc',
      playerVars: {
        autoplay: 1
      }
    }
  },
  methods: {
    playing() {
    //   console.log('\o/ we are watching!!!')
    }
  }
}
</script>

<style scoped>

</style>