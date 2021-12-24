<template>
  <div class="card">
    <div class="row px-2">
      <img :src="datos.img" alt="" />
    </div>
    <div class="row px-3 reducir">
      <div class="col">
        {{ datos.description }}
      </div>
    </div>
    <div class="row px-2 d-flex justify-content-end">
      <div class="col-4 aumentar">
        <strong> ${{ datos.precio }}</strong>
      </div>
    </div>
    <div class="row mb-3 d-flex justify-content-end">
      <div class="col-4 reducir-2 reducir-2">$6.75</div>
    </div>
  </div>
</template>
<script>
export default {
  name: "card",
  props: {
    datos: Array,
  },
};
</script>
<style scoped>
.reducir {
  font-size: 15px;
}

.reducir-2 {
  font-size: 15px;
  text-decoration: line-through;
}

.aumentar {
  font-size: 20px;
  color: rgb(0, 150, 161);
}
</style>