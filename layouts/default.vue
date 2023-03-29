<template>
  <v-app>
    <v-main>
      <v-sheet color="primary">
        <v-container class="pa-0">
          <v-app-bar flat color="primary">
            <figure class="img__container d-flex align-center">
              <img src="~/static/logo.png" height="45px" />
            </figure>
            <v-spacer></v-spacer>
            <div
              class="img__container d-flex align-end"
              v-if="this.$vuetify.breakpoint.mdAndUp"
            >
              <v-tabs
                dark
                background-color="primary"
                active-class="menu__btn-active"
              >
                <v-tabs-slider color="accent"></v-tabs-slider>
                <v-tab :ripple="false" @click="scrollTo('services')"
                  >Servicios</v-tab
                >
                <v-tab :ripple="false" @click="scrollTo('about-us')"
                  >Nosotros</v-tab
                >
                <v-tab :ripple="false" @click="scrollTo('clients')"
                  >Clientes</v-tab
                >
                <v-tab :ripple="false">Contáctanos</v-tab>
              </v-tabs>
            </div>
          </v-app-bar>
        </v-container>
      </v-sheet>
      <Nuxt />
    </v-main>
    <footer>
      <v-container>
        <v-row>
          <v-col cols="12" xs="12" sm="12" md="6">
            <p class="footer__title mb-0">Dirección:</p>
            <p class="footer__text">
              Providencia, Col. Del Valle Centro, CP 03100, CDMX
            </p>
            <p class="footer__title mb-0">Teléfonos:</p>
            <!-- <p class="footer__text mb-0">(+01) 123-456-78-90</p> -->
            <p class="footer__text mb-0">(+52) 554-003-22-76</p>
          </v-col>
          <v-col cols="12" xs="12" sm="12" md="6" class="footer__social">
            <v-btn icon large class="footer__social--icon"
              ><v-icon color="#fff">mdi-facebook</v-icon></v-btn
            >
            <v-btn icon large class="footer__social--icon">
              <v-icon color="#fff">mdi-instagram</v-icon>
            </v-btn>
          </v-col>
        </v-row>
      </v-container>
    </footer>
  </v-app>
</template>

<script>
export default {
  name: "DefaultLayout",
  data() {
    return {};
  },
  methods: {
    scrollTo(to) {
      const element = document.getElementById(to);
      element.scrollIntoView({ block: "start", behavior: "smooth" });
    },
  },
};
</script>

<style lang="scss">
.v-toolbar__content {
  padding: 0px;
}

.v-tab {
  color: #ffffff !important;
  text-transform: none;
  font-family: "Rubik";
  font-weight: 400;
}

.menu__btn-active {
  color: #ffdd3f !important;
  background-color: #415364 !important;
  font-weight: 500;
}

.v-tab--active.v-tab:not(:focus)::before {
  opacity: 0;
  color: transparent;
  background-color: transparent;
}

.img__container {
  height: 100%;
}

footer {
  background-color: #415364;
  padding-top: 2rem;
  padding-block: 1.5rem;
}

.footer__title {
  font-family: "Karla";
  font-style: normal;
  font-weight: 500;
  color: #ffdd3f;
}

.footer__text {
  font-family: "Karla";
  font-style: normal;
  font-weight: 500;
  line-height: 25px;
  color: #ffffff;
}

.footer__social {
  display: flex;
  align-items: flex-end;
  justify-content: flex-end;
}

.footer__social--icon {
  background-color: #68c3cd;
  margin-right: 1rem;
}

@media only screen and (max-width: 959px) {
  .footer__social {
    display: flex;
    align-items: flex-start;
    justify-content: flex-start;
  }

  .footer__social--icon {
    background-color: #68c3cd;
    margin-right: 1rem;
  }
}
</style>