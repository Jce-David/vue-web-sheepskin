<script lang="ts" >
import TopBar from './components/TopBar.vue';
import ProductMain from './components/ProductMain.vue';
import TopBarLogo from './components/TopBarLogo.vue'
import TopBarWithLogo from './components/TopBarWithLogo.vue'
import TopBar2 from './components/TopBar2.vue';
export default {
    components: { TopBar, TopBarLogo, TopBar2 },
    data(){ 
      return {

      }
    }
}
</script>

<template>
   <v-app id="inspire"  >
    <v-app-bar   height="120" v-if="$route.name === 'home'" app elevation="0" >
      <TopBarLogo />
    </v-app-bar>
    <v-app-bar   >
      <TopBar class=" d-none d-sm-flex " />
      <TopBar2 class="d-none d-lg-flex" />
    </v-app-bar>
    <v-main  class="bg-grey-lighten-3" >
     <RouterView />>
    </v-main>
  </v-app>
</template>