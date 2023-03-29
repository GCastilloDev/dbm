<template>
  <v-container>
    <v-row>
      <v-col
        class="d-flex align-center"
        cols="12"
        xs="12"
        sm="12"
        md="6"
        order="2"
        order-md="1"
      >
        <div>
          <h2 class="banner__title">
            LA MEJOR GUÍA PARA TÚ <span>E-COMMERCE</span>
          </h2>
          <p class="banner__slogan">
            Te brindamos asesoría de principio a fin para crear tu e-commerce e incrementar tus ventas hasta un 25%.
          </p>
          <v-btn color="primary" outlined>CONTÁCTANOS</v-btn>
        </div>
      </v-col>
      <v-col cols="12" xs="12" sm="12" md="6" order="1" order-md="2">
        <figure class="banner__img d-flex align-center justify-center">
          <img src="~/static/banner.png" width="80%" alt="banner image" />
        </figure>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Banner",
};
</script>

<style lang="css">
.banner__title {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 500;
  font-size: 45px;
  line-height: 64px;
  color: #415364;
}

.banner__title > span {
  padding-right: 0.3rem;
  padding-left: 0.3rem;
  color: #ffff;
  background: #68c3cd;
}

.banner__slogan {
  font-family: "Karla";
  font-style: normal;
  font-weight: 500;
  line-height: 32px;
  color: #97afb2;
  margin-bottom: 0px;
}

.banner__img {
  width: 100%;
}

.v-btn {
  letter-spacing: 0.05em;
}
</style>