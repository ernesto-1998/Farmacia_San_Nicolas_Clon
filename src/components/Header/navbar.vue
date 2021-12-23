<template>
  <div class="nav">
    <div class="navbar-content">
      <ul class="navbar-content-left">
        <li>
          <router-link to="#" class="routerlink btn">
            <i class="bx bxs-grid bx-sm"></i>
            <span>productos por categoría</span>
          </router-link>
        </li>
        <li>
          <router-link to="#" class="routerlink btn">
            <i class="bx bx-purchase-tag-alt bx-sm"></i>
            <span>Promociones</span>
          </router-link>
        </li>
        <li>
          <router-link to="#" class="routerlink btn">
            <i class="bx bxs-file-doc bx-sm"></i>
            <span>Comprar con receta</span>
          </router-link>
        </li>
        <li>
          <router-link to="#" class="routerlink btn">
            <i class="bx bx-bookmark-plus bx-sm"></i>
            <span>Comprar con seguro</span>
          </router-link>
        </li>
      </ul>
      <div class="navbar-content-right">
        <input type="text">
        <router-link to="#">
          <i class="bx bx-cart bx-md"></i>
        </router-link>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "navbar",
};
</script>
<style scoped>
* {
  box-sizing: border-box;
  background-color: rgb(0, 150, 161);
}

a {
  color: #fff;
}

span {
  /* color: #fff; */
  text-transform: uppercase;
  font-size: 13px;
}

ul {
  list-style: none;
  height: 100%;
}
.nav {
  width: 100%;
}

.nav ul {
  display: flex;
  align-items: center;
}

.navbar-content {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  justify-content: space-between;
}

.navbar-content-left li {
  border-right: 1px solid #fff;
  padding: 5px 0;
}

.navbar-content-left :last-child {
  border: none;
}

.navbar-content-right {
  display: flex;
  align-items: center;
  color: #fff;
  padding: 12px 0;
}

.navbar-content-right input {
  background-color: #fff;
  border: none;
  width: 400px;
  margin-right: 10px;
  border-radius: 5px;
  height: 100%;
}

.routerlink {
  display: flex;
  align-items: center;
}
</style>