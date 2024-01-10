<template>
  <header class="header-container">
    <!-- Immagine di sfondo e logo -->
<div class="top-bar">
      <div class="logo-container">
      <img src="../assets/img/gym_logo_2x.png" alt="Logo" class="img-fluid logo-header">
    </div>

    <!-- Menu con voci popolate dinamicamente -->
    <nav>
      <ul class="navbar-nav">
        <li v-for="item in menuItems" :key="item.id" class="nav-item">
          <a class="nav-link" href="#">{{ item.label }}</a>
        </li>
      </ul>
    </nav>
  </div>


    <div class="header-content">
      <h1 class="text-center">NO PAIN NO GAIN</h1>
      <button class="btn btn-primary">JOIN US TODAY</button>
    </div>






  </header>
</template>

<script>
export default {
  props: {
    menuItems: Array,
  },
};
</script>

<style>
/* Aggiungi stili specifici per l'header */

.logo-container {
width: 20%;
}
.header-container {
  display: flex;
  flex-direction: column;

  justify-content: space-between;
  padding: 20px;
  background-color: #333; /* Aggiungi il colore di sfondo desiderato */
  color: white;
  width: 100%;
  height: 600px;
}

.header-background {
  height: 600px;
  width: 100%;
}

.logo-header {
  width: 100%;
}

.top-bar{
  display: flex;
  flex-direction: row;
  width: 100%;
}

.navbar-nav {
  display: flex;
  flex-direction: row;
  width: 80%;
  list-style: none;
  margin: 0;
  padding: 0;
}

.nav-item {
  margin-right: 15px;
}

.nav-link {
  text-decoration: none;
  color: white;
}

.header-content {
  text-align: center;
}

</style>
