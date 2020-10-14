<template>
  <section class="pb-8 mt-5" id="contact">
    <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row justify="center">
            <v-col cols="12" sm="5">
              <h1 class="font-weight-light display-1">Contactenos</h1>
              <h3 class="font-weight-light mt-3">
                Contáctenos por chat de WhatsApp , por teléfono o Email y realiza consultas online de forma fácil y rápida: problemas técnicos , presupuestos , formas pagos y otras consultas.
                Recibi asesoramiento del equipo técnico del Taller.
              </h3>
              <h3 class="font-weight-light mt-3">
                Lorem ipsum dolor sit amet consectetur adipisicing.
              </h3>
              <h3 class="font-weight-light mt-3">
                Telefono: +261 xxx-xxxx
              </h3>
              <h3 class="font-weight-light">
                Email: email@email.com
              </h3>
            </v-col>
            <v-col cols="12" sm="7">
              <v-form ref="form" v-model="valid" :lazy-validation="lazy">
                <v-text-field
                  v-model="name"
                  :counter="10"
                  :rules="nameRules"
                  label="Nombre"
                  required
                ></v-text-field>

                <v-text-field
                  v-model="email"
                  :rules="emailRules"
                  label="E-mail"
                  required
                ></v-text-field>

                <v-textarea
                  v-model="textArea"
                  :rules="textAreaRules"
                  label="Mensage"
                  required
                />

                <v-btn
                  :disabled="!valid"
                  color="primary"
                  :dark="valid"
                  rounded
                  block
                  class="mt-3"
                >
                  Enviar
                </v-btn>
              </v-form>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
    <div class="svg-border-waves text-white">
      <v-img src="~@/assets/img/borderWavesBlue.svg" />
    </div>
  </section>
</template>

<style scoped>
#contact {
  background-color: #f4f7f5;
}

.svg-border-waves .v-image {
  position: absolute;
  bottom: 0;
  left: 0;
  height: 3rem;
  width: 100%;
  overflow: hidden;
}

</style>

<script>
export default {
  data: () => ({
    icons: ["fa-facebook", "fa-twitter", "fa-linkedin", "fa-instagram"],
    valid: true,
    name: "",
    nameRules: [
      (v) => !!v || "Este campo es obligatorio",
      (v) => (v && v.length >= 4) || "Manimo 4 caracteres",
    ],
    email: "",
    emailRules: [
      (v) => !!v || "Este campo es obligatorio",
      (v) => /.+@.+\..+/.test(v) || "El email debe ser valido",
    ],
    textArea: "",
    textAreaRules: [
      (v) => !!v || "Este campo es obligatorio",
      (v) => (v && v.length >= 10) || "Mínimo de 10 caracteres",
    ],
    lazy: false,
  }),
};
</script>
