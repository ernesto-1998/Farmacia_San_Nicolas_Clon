<template>
  <div class="home">
    <cabecera/>
    <navbar/>
    <carousel/>
  </div>
</template>

<script>
// @ is an alias to /src

import cabecera from '../components/Header/head';
import navbar from '../components/Header/navbar';
import carousel from '../components/Carousel/carousel';

export default {
  name: 'Home',
  components: {
    cabecera,
    navbar,
    carousel
    
  }
}
</script>
