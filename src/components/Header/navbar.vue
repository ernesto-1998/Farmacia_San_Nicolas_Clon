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
        <!-- <input type="text" placeholder="Buscar producto"> -->
        <div class="input-group">
          <input type="text" class="form-control backwhite" placeholder="Buscar producto" aria-label="Recipient's username" aria-describedby="button-addon2">
          <button class="btn btn-outline-secondary backwhite" type="button" id="button-addon2"><i class='bx bx-search bx-sm backwhite'></i></button>
        </div>        
        <router-link to="#">
          <i class="bx bx-cart bx-md px-3"></i>
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
  text-transform: uppercase;
  font-size: 12px;
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
  padding: 2px 0;
}

.navbar-content-left :last-child {
  border: none;
}

.navbar-content-right {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  color: #fff;
  padding: 12px 0;
  width: 100%;
}

.backwhite{
  background-color: #fff;
}

.input-group button {
  border-left: none;
}

.routerlink {
  display: flex;
  align-items: center;
}
</style>