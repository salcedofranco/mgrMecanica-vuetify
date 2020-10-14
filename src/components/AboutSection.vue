<template>
  <section id="about">
    <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row align="center" justify="center">
            <v-col cols="12" md="7">
              <h1 class="font-weight-light display-2">Nosotros</h1>
              <h1 class="font-weight-light display-1 mb-3">
                Lorem ipsum dolor!
              </h1>
              <v-row>
                <v-col cols="12" class="d-flex align-center">
                  <v-img
                    src="@/assets/img/auto1.png"
                    max-width="60px"
                    class="mr-4"
                  />
                  <p class="text-justify">
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                  </p>
                </v-col>
                <v-col cols="12" class="d-flex align-center">
                  <v-img
                    src="@/assets/img/auto.png"
                    max-width="60px"
                    class="mr-4"
                  />
                  <p class="text-justify">
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                  </p>
                </v-col>
                <v-col cols="12" class="d-flex align-center">
                  <v-img
                    src="@/assets/img/limpieza.png"
                    max-width="60px"
                    class="mr-4"
                  />
                  <p class="text-justify">
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                  </p>
                </v-col>
              </v-row>
            </v-col>
            <v-col cols="12" md="5" class="d-none d-md-flex">
              <v-img
                src="@/assets/img/taller2.jpg"
                class="d-block ml-auto mr-auto"
                max-width="400px"
              />
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
#about {
  background-color: #f3f4f5;
}
</style>
