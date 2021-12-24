<template>
  <div class="nav">
    <div class="nav-content">
      <div class="nav-brand">
        <router-link to="#">
          <img src="../../assets/logo.svg" alt="Farmacia San Nicolas" />
        </router-link>
      </div>
      <ul class="nav-content-right">
        <li>
            <router-link class="routerlink" to="#">
                <i class='bx bx-credit-card bx-sm'></i>
                <span>Club VIP</span>
            </router-link>
        </li>
        <li>
          <div class="dropdown">
            <a
              class="dropdown-toggle routerlink"
              type="button"
              id="dropdownMenuButton1"
              data-bs-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
            <i class='bx bx-plus-circle bx-sm'></i>
              <span>Conózcanos</span>
            </a>
            <div class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
              <a class="dropdown-item" href="#">¿Quiénes somos?</a>
              <a class="dropdown-item" href="#">Conózcanos</a>
            </div>
          </div>
        </li>
        <li>
          <div class="dropdown">
            <a
              class="dropdown-toggle routerlink"
              type="button"
              id="dropdownMenuButton2"
              data-bs-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
            <i class='bx bx-injection bx-sm' ></i>
              <span>Servicios</span>
            </a>
            <div class="dropdown-menu" aria-labelledby="dropdownMenuButton2">
              <a class="dropdown-item" href="#">Nuestros servicios</a>
              <a class="dropdown-item" href="#">Jornadas de salud</a>
              <a class="dropdown-item" href="#">Blog de salud</a>
              <a class="dropdown-item" href="#">Revista San Nicolás</a>
              <a class="dropdown-item" href="#">Red de médicos</a>
            </div>
          </div>            
        </li>
        <li>
            <router-link to="#" class="routerlink">
                <i class='bx bx-map bx-sm'></i>
                <span>Sucursales</span>
            </router-link>
        </li>
        <li>
          <div class="dropdown">
            <a
              class="dropdown-toggle routerlink"
              type="button"
              id="dropdownMenuButton3"
              data-bs-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
            <i class='bx bx-user bx-sm'></i>
              <span>Ingresar</span>
            </a>
            <div class="dropdown-menu" aria-labelledby="dropdownMenuButton3">
              <a class="dropdown-item" href="#">Iniciar Sesión</a>
              <a class="dropdown-item" href="#">Registrarme</a>
            </div>
          </div>            
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  name: "cabecera",
};
</script>
<style scoped>
* {
  box-sizing: border-box;
}

a {
  color: rgb(73, 73, 73);
}

ul {
  list-style: none;
  height: 100%;
}

img {
  max-width: 100%;
}

.routerlink {
    text-decoration: none;
    display: flex;
    align-items: center;
}

.nav {
  width: 100%;
  height: auto;
  padding: 15px 10px;
  background-color: #fff;
  max-width: 1440px;
  box-shadow: 0 1px 3px rgb(0 0 0 / 10%), 0 2px 2px rgb(0 0 0 / 6%),
    0 0 2px rgb(0 0 0 / 7%);
}

.nav-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
}

.nav ul {
  display: flex;
  align-items: center;
  margin: 0;
  padding: 0;
}

.nav li {
  margin: 0 15px;
  font-size: 13px;
}

.nav-content-right span {
    text-decoration: underline;
    margin-left: 5px;
    display: flex;
    align-items: center;
}

.nav li :hover {
    color: rgb(236, 0, 138);
}

.nav-brand img {
  width: 350px;
}

@media(max-width: 768px){
    .nav {
        display: none;
    }
}
</style>