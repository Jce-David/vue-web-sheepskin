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
    
      <RouterLink custom v-slot="{ navigate }" to="/"> <v-btn :active="$route.name === 'home'" variant="text"
          @click="navigate">  
          <span class="d-block pa-2" >
            Home
          </span>
        </v-btn>
      </RouterLink>
   
    
      <RouterLink custom v-slot="{ navigate }" to="/product"> <v-btn :active="$route.name === 'product'" variant="text"
          @click="navigate">
          <span class="d-block pa-2"  >
            Productos
          </span>
       </v-btn>
      </RouterLink>

   
    
      <RouterLink custom v-slot="{ navigate }" to="/nosotros"> <v-btn :active="$route.name === 'nosotros'" variant="text"
          @click="navigate">
          <span class="d-block pa-2"  >
            Nosotros
          </span>
        </v-btn>
      </RouterLink>
      
   
     
      
        <RouterLink custom v-slot="{ navigate }" to="/soporte"> <v-btn :active="$route.name === 'soporte'" variant="text"
          @click="navigate">
          <span class="d-block pa-2"  >
            Soporte
          </span>
        </v-btn>
      </RouterLink>
     
  </v-row>
</v-container>
</template>
