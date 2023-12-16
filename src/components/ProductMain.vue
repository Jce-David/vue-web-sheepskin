<script lang="ts">

export default {

}
</script>

<template>
  <v-carousel class="hidden-sm-and-down">
    <v-carousel-item>
      <v-img cover class="d-flex align-center justify-center text-white"
        src="https://lahormadetunegocio.com/wp-content/uploads/2020/10/Importancia-del-Control-de-Calidad-en-la-Industria-del-Calzado.-.jpg">
        <p class="text-h3 text-center">Producto 100% Peruano</p>

        <v-card-actions class=" d-flex justify-center">
          <router-link v-slot="{ navigate }" custom to="/product">
            <v-btn @click="navigate" variant="outlined">
              <p class="my-class text-center">Ver Productos</p>
            </v-btn>
          </router-link>
        </v-card-actions>
      </v-img>
    </v-carousel-item>



    <v-carousel-item>
      <v-img cover class="d-flex align-center justify-center text-white"
        src="https://www.clinicauandes.cl/images/default-source/resize/buen-uso-de-calzado-940x430_08072019.jpg">

        <p class="text-h3 text-center"> Productos de calidad </p>

        <v-card-actions class=" mt-4  d-flex justify-center">
          <router-link custom v-slot="{ navigate }" to="/product">
            <v-btn @click="navigate" variant="outlined">
              <p class="my-class text-center">
                Ver Productos</p>
            </v-btn> </router-link>

        </v-card-actions>
      </v-img>
    </v-carousel-item>
    <v-carousel-item>
      <v-img cover class="d-flex align-center justify-center text-white"
        src="https://canadianjohn.es/wp-content/uploads/2023/03/calzado-calida-980x551.jpg">

        <p class="text-h3 text-center">Hecho a mano</p>

        <v-card-actions class=" mt-4  d-flex justify-center">
          <router-link custom v-slot="{ navigate }" to="/product">
            <v-btn @click="navigate" variant="outlined">
              <p class="my-class text-center">Ver Productos</p>
            </v-btn>
          </router-link>
        </v-card-actions>
      </v-img>
    </v-carousel-item>
  </v-carousel>

  <v-card class="hidden-md-and-up">

    <v-card>
      <v-img cover class="d-flex align-center justify-center text-white"
        src="https://lahormadetunegocio.com/wp-content/uploads/2020/10/Importancia-del-Control-de-Calidad-en-la-Industria-del-Calzado.-.jpg">
      </v-img>
    </v-card>
    <v-card>
      <v-img cover class="d-flex align-center justify-center text-white"
        src="https://www.clinicauandes.cl/images/default-source/resize/buen-uso-de-calzado-940x430_08072019.jpg">
      </v-img>
    </v-card>
    <v-card>
      <v-img cover class="d-flex align-center justify-center text-white"
        src="https://canadianjohn.es/wp-content/uploads/2023/03/calzado-calida-980x551.jpg">
      </v-img>
    </v-card>
  </v-card>
</template>