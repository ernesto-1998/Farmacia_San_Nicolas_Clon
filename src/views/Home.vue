<template>
  <div class="home">
    <cabecera />
    <navbar />
    <carousel />
    <div class="contenedor">
      <div class="content">
        <div class="division">promos especiales</div>
        <div class="row">
          <div class="col-3 mb-4" v-for="(value, index) in datos" :key="index">
            <card :datos="value" />
          </div>
        </div>
        <div class="row d-flex justify-content-center">
          <div class="col-3 mb-5">
            <router-link to="#" class="btn background py-2 w-100">
              <i class="bx bx-plus-medical me-2"></i>
              <Strong><span>Ver más</span></Strong>
            </router-link>
          </div>
        </div>
      </div>
    </div>
    <div class="banner-container">
      <div class="wrap container-fluid">
        <img src="../assets/Bannerbajo.jpg" alt="">
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import cabecera from "../components/Header/head";
import navbar from "../components/Header/navbar";
import carousel from "../components/Carousel/carousel";
import card from "../components/Cards/card";

export default {
  name: "Home",
  components: {
    cabecera,
    navbar,
    carousel,
    card,
  },
  data() {
    return {
      datos: [
        {
          img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg",
          description:
            "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA",
          precio: 3.75,
        },
        {
          img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg",
          description:
            "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA",
          precio: 3.75,
        },
        {
          img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg",
          description:
            "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA",
          precio: 3.75,
        },
        {
          img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg",
          description:
            "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA",
          precio: 3.75,
        },
        {
          img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg",
          description:
            "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA",
          precio: 3.75,
        },
        {
          img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg",
          description:
            "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA",
          precio: 3.75,
        },
        {
          img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg",
          description:
            "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA",
          precio: 3.75,
        },
        {
          img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg",
          description:
            "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA",
          precio: 3.75,
        },
      ],
    };
  },
};
</script>

<style scoped>
a {
  text-decoration: none;
  color: #fff;
}

.wrap img {
    max-width: 100%;
    max-height: 100%;
    display: block;
    margin: 25px 0;
}

.wrap {
  display: flex;
  justify-content: center;
  padding: 0 25px;
}

.contenedor{
  width: 100%;
  height: auto;
  background-color: rgb(242, 242, 242);
}

.content {
  margin: 0 25px;
}

.division {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: auto;
  text-transform: uppercase;
  color: #fff;
  background-color: rgb(32, 51, 56);
  font-size: 40px;
  /* margin: 45px 0; */
  margin-top: 45px;
  margin-bottom: 30px;
  border-radius: 25px;
}

.background {
  background-color: rgb(236, 0, 138);
  color: #fff;
  border-radius: 25px;
  font-size: 20px;
}

.banner-container{
  width: 100%;

}

</style>
