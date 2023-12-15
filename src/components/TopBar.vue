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
  <v-spacer></v-spacer>
  <RouterLink custom v-slot="{ navigate }" to="/"> <v-btn 
      :active="$route.name === 'home'" variant="text" @click="navigate">Home</v-btn>
  </RouterLink>
  <RouterLink custom v-slot="{ navigate }" to="/product"> <v-btn 
      :active="$route.name === 'product'" variant="text" @click="navigate">Productos</v-btn>
  </RouterLink>
  <RouterLink custom v-slot="{ navigate }" to="/nosotros"> <v-btn 
      :active="$route.name === 'nosotros' " variant="text" @click="navigate">Nosotros</v-btn>
  </RouterLink>
  <RouterLink custom v-slot="{ navigate }" to="/soporte"> <v-btn 
      :active="$route.name === 'soporte' " variant="text" @click="navigate">Soporte</v-btn>
  </RouterLink>
  
          <v-spacer></v-spacer>
</template>
