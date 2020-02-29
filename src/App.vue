<template>
  <v-app>
  <ToolBar />
    
      <router-view></router-view>
   
  </v-app>
</template>

<script>
import ToolBar from '@/components/ToolBar';
export default {
  name: 'App',
  components :{ToolBar},
 
  data: () => ({
    //
  }),
};
</script>
