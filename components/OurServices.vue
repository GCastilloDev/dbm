<template>
  <section>
    <header class="services__header">
      <v-container>
        <h3 class="title__section"><span>NUES</span>TROS SERVICIOS</h3>
      </v-container>
    </header>
    <v-container class="services__cards">
      
      <v-row class="services__card--container pb-15" justify="space-around">
        <v-col cols="12" xs="12" sm="12" md="4">
          <v-card class="card__container" outlined>
            <v-card-text>
              <figure class="card__img">
                <img
                  src="~/static/card_img_2.png"
                  alt="Gestión del acta constitutiva de tu empresa"
                  width="100%"
                />
              </figure>
              <h4 class="card__title">
                Servicios de E-comerce:
              </h4>
              <ul class="card__list">
                <li>Gestión y aperturas de tus cuentas Seller Central en  Amazon y Mercado Libre. Seller Central representa  venta a través de Amazon.</li>
                <li>Abrimos y gestionamos tus cuentas Vendor Central (sólo para dueños de marca). Vendor Central representa ventas a Amazon.</li>
                <li>Te ayudamos con tus Estrategias de comercialización de nuevos productos. Creamos para ti las estrategias de Marketing para posicionamiento de productos en línea.</li>
                <li>Damos seguimiento de las ventas en plataformas electrónicas.</li>
                <li>Corregimos defectos en la cadena de suministro y verificamos conformidad con los criterios de entrega y empaquetado.</li>
              </ul>
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" xs="12" sm="12" md="4">
          <v-card class="card__container" outlined>
            <v-card-text>
              <figure class="card__img">
                <img
                  src="~/static/card_img_1.png"
                  alt="Gestión del acta constitutiva de tu empresa"
                  width="100%"
                />
              </figure>
              <h4 class="card__title">
                Gestión del acta constitutiva de tu empresa
              </h4>
              <ul class="card__list">
                <li>Búsqueda y registro de la razón social.</li>
                <li>La conformación de los estatutos.</li>
                <li>Gestiones con el notario.</li>
                <li>Representación legal.</li>
                <li>Asesoría fiscal.</li>
              </ul>
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" xs="12" sm="12" md="4">
          <v-card class="card__container" outlined>
            <v-card-text>
              <figure class="card__img">
                <img
                  src="~/static/card_img_2.png"
                  alt="Asesoría legal para venta en línea"
                  width="100%"
                />
              </figure>
              <h4 class="card__title">Asesoría legal para venta en línea</h4>
              <ul class="card__list">
                <li>Registro de marca.</li>
                <li>Aviso de privacidad.</li>
                <li>Patentes.</li>
                <li>Propiedad intelectual.</li>
              </ul>
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" xs="12" sm="12" md="4">
          <v-card class="card__container" outlined>
            <v-card-text>
              <figure class="card__img">
                <img
                  src="~/static/card_img_3.png"
                  alt="Asesoría legal corporativa"
                  width="100%"
                />
              </figure>
              <h4 class="card__title">Asesoría legal corporativa</h4>
              <ul class="card__list">
                <li>
                  Contratos de compraventa, prestaciones de servicios
                  profesionales, arrendamientos.
                </li>
                <li>
                  Contratos para proveedores, suministro, comisión mercantil,
                  licencia de marca.
                </li>
                <li>
                  Contratos laborales, temporales, tiempo indeterminado,
                  capacitación inicial y periodo de prueba.
                </li>
              </ul>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  name: "OurServices",
};
</script>

<style lang="css" scoped>
.services__header {
  background-color: #f3f7f9;
  height: 150px;
}

.card__container {
  background-color: transparent;
  border: 2px solid #97afb2;
  box-sizing: border-box;
  filter: drop-shadow(4px 4px 20px rgba(0, 0, 0, 0.15));
  border-radius: 12px;
  height: 100%;
}

.card__img {
  width: 100%;
}

.card__title {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 500;
  font-size: 21px;
  line-height: 32px;
  color: #415364;
}

.card__list {
  margin-top: 1rem;
  font-family: "Karla";
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  color: #61788e;
}

.services__card--container {
  background-image: url("~/static/dots.png");
  background-position: right bottom;
  background-repeat: no-repeat;
}

.services__cards {
  margin-top: -70px;
}

@media only screen and (max-width: 959px) {
  .services__header {
    height: 200px;
  }
}
</style>