<template>
  <div class="home">
    <cabecera />
    <navbar />
    <carousel />
    <div class="content">
      <div class="division">promos especiales</div>
      <div class="row">
        <div class="col-3 mb-4" v-for="(value, index) in datos" :key="index">
          <card :datos="value"/>
        </div>
      </div>
      <div class="row d-flex justify-content-center mb-4">
        <div class="col-3 background py-2">
          <router-link to="#">
            <i class='bx bx-plus-medical me-2'></i>
            <Strong><span>Ver más</span></Strong>
          </router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import cabecera from "../components/Header/head";
import navbar from "../components/Header/navbar";
import carousel from "../components/Carousel/carousel";
import card from '../components/Cards/card';

export default {
  name: "Home",
  components: {
    cabecera,
    navbar,
    carousel,
    card
  },
  data(){
    return {
      datos: [
        {img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg", description: "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA", precio: 3.75},
        {img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg", description: "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA", precio: 3.75},
        {img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg", description: "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA", precio: 3.75},
        {img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg", description: "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA", precio: 3.75},
        {img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg", description: "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA", precio: 3.75},
        {img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg", description: "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA", precio: 3.75},
        {img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg", description: "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA", precio: 3.75},
        {img: "https://www.disfarma.com.co/fotosproductos/main_producto_3.jpg", description: "EL PRODUCTO PRO EXCELENCIA EN LO QUE A CURA DE MALESTAR RESPECTA", precio: 3.75}
      ]
    }
  }
};
</script>

<style scoped>

a {
  text-decoration: none;
  color: #fff;
}

.content{
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

.background{
  background-color: rgb(236, 0, 138);
  color: #fff;
  border-radius: 25px;
  font-size: 20px;
  
}
</style>
