<template>
  <section id="marcas">
    <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row align="center" justify="center">
            <v-col sm="4" class="hidden-xs-only">
              <v-img src="@/assets/img/taller.jpg" class="d-block ml-auto mr-auto" max-width="350px" />
            </v-col>
            <v-col cols="12" sm="8" class="white--text text-left">
              <h1 class="font-weight-light display-2 mb-2">TRABAJAMOS TODAS LAS MARCAS</h1>
              <h1 class="font-weight-light">
                Nuestro Taller Mecánico Automotriz cuenta con personal capacitado en
                todas las marcas, modernas instalaciones, equipamiento de primera,
                y el mejor servicio personalizado de Mendoza.
                Nuestra premisa es brindarte calidad y garantía de servicio.
              </h1>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
#marcas {
  background-image: url("~@/assets/img/bgMecanica2.jpg");
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  height: 500px;
}

#marcas .container,
#marcas .row {
  height: 100%;
}
</style>
