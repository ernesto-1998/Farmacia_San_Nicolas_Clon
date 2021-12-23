<template>
  <div class="home">
    <cabecera/>
    <navbar/>
  </div>
</template>

<script>
// @ is an alias to /src

import cabecera from '../components/Header/head';
import navbar from '../components/Header/navbar';

export default {
  name: 'Home',
  components: {
    cabecera,
    navbar
    
  }
}
</script>
