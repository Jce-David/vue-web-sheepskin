<script lang="ts" >
import TopBar from './components/TopBar.vue';
import ProductMain from './components/ProductMain.vue';
import TopBarLogo from './components/TopBarLogo.vue'
import TopBarWithLogo from './components/TopBarWithLogo.vue'
export default {
    components: { TopBar, TopBarLogo, TopBarWithLogo }
}
</script>

<template>
   <v-app id="inspire"  >
    <v-app-bar v-if="$route.name === 'home'"  app elevation="0" >
      <TopBarLogo />
    </v-app-bar>
    <v-app-bar v-if="$route.name === 'home'" color="red" class="px-3"
      flat
      density="compact" >
      <TopBar />
    </v-app-bar>
    <v-app-bar v-else color="red" class="px-3"
      flat
      density="compact" >
      <TopBarWithLogo />
    </v-app-bar>
    <v-main class="bg-grey-lighten-3" >
     <RouterView />>
    </v-main>
  </v-app>
</template>