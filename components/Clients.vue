<template>
  <v-container>
    <h3 class="title__section mb-10"><span>CLIEN</span>TES SATISFECHOS</h3>
    <v-row justify="center">
      <v-col cols="12" xs="12" sm="12" md="8">
        <v-carousel
          class="pb-15"
          v-model="model"
          height="100%"
          progress-color="#68c3cd"
          cycle
          :show-arrows="false"
        >
          <v-carousel-item v-for="i in 6" :key="i">
            <div class="d-flex align-center px-16" style="height: 100%">
              <v-card class="py-5 px-3" outlined>
                <v-row>
                  <v-col
                    class="d-flex align-center justify-center"
                    cols="12"
                    xs="12"
                    sm="12"
                    md="4"
                  >
                    <v-avatar size="120">
                      <img
                        src="https://cdn.vuetifyjs.com/images/john.jpg"
                        alt="John"
                      />
                    </v-avatar>
                  </v-col>
                  <v-col cols="12" xs="12" sm="12" md="8">
                    <p class="client__title">Lorem ipsum dolor</p>
                    <p class="mb-0 client__text">
                      Lorem ipsum dolor sit amet, consectetur adipiscing elit,
                      sed do eiusmod tempor incididunt ut labore et dolore magna
                      aliqua.
                    </p>
                  </v-col>
                </v-row>
              </v-card>
            </div>
          </v-carousel-item>
        </v-carousel>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Clients",

  data: () => ({
    model: 0,
  }),
};
</script>

<style lang="css">
.client__title {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  line-height: 28px;
  color: #68c3cd;
}

.client__text {
  font-family: "Karla";
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  color: #61788e;
}

.v-carousel__controls {
  background: rgba(104, 195, 205, 0.5) !important;
}
</style>