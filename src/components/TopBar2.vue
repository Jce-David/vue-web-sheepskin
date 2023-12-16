<script lang="ts">

export default {
  data() {
    return {
      links: [
        'Inicio',
        'Productos',
        'Soporte',
        'Nosotros',
      ]
    }
  }
}

</script>

<template>
<v-container >
  <v-row class="d-flex justify-center align-center"  >
    
      <RouterLink custom v-slot="{ navigate }" to="/"> 
        <v-btn icon="mdi-home" :active="$route.name === 'home'" variant="text"
          @click="navigate">  
        
        </v-btn>
      </RouterLink>
   
    
      <RouterLink custom v-slot="{ navigate }" to="/product"> <v-btn :active="$route.name === 'product'" variant="text"
          @click="navigate">
          <v-icon icon="mdi-cart" ></v-icon>
       </v-btn>
      </RouterLink>

   
    
      <RouterLink custom v-slot="{ navigate }" to="/nosotros"> <v-btn :active="$route.name === 'nosotros'" variant="text"
          @click="navigate">
          <v-icon icon="mdi-about" ></v-icon>
        </v-btn>
      </RouterLink>
      
   
     
      
        <RouterLink custom v-slot="{ navigate }" to="/soporte"> <v-btn :active="$route.name === 'soporte'" variant="text"
          @click="navigate">
          <v-icon icon="mdi-" ></v-icon>
        </v-btn>
      </RouterLink>
     
  </v-row>
</v-container>
</template>
