<template>
    <div class="nav">
        <div class="nav-content">
            <div class="nav-brand">
                <router-link to="#">
                    <img src="../../assets/logo.svg" alt="Farmacia San Nicolas">
                </router-link>
            </div>
            <ul class="nav-content-right">
                <li><router-link to="#">Club VIP</router-link></li>
                <li><router-link to="#">Conozcanos</router-link></li>
                <li><router-link to="#">Servicios</router-link></li>
                <li><router-link to="#">Servicios</router-link></li>
                <li><router-link to="#">Ingresar</router-link></li>
            </ul>
        </div>
        
    </div>
</template>
<script>
export default {
    name: 'cabecera'
}
</script>
<style scoped>

    * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }

    a {
        color: rgb(73, 73, 73);
    }

    ul {
        list-style: none;
    }

    img {
        max-width: 100%;
    }   

    .nav{
        width: 100%;
        height: auto;
        padding: 15px 10px;
        background-color: #fff;
        box-shadow: 0 1px 3px rgb(0 0 0 / 10%), 0 2px 2px rgb(0 0 0 / 6%),
        0 0 2px rgb(0 0 0 / 7%);
    }

    .nav-content{
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        align-items: center;
        max-width: 1440px;
        margin: 0 auto;
    }

    .nav-brand {
        display: flex;
        justify-content: start;
    }

    .nav ul {
        display: flex;
        align-items: center;
    }

    .nav li {
        margin: 0 15px;
    }

    .nav-brand img {
        width: 320px;
    }
</style>