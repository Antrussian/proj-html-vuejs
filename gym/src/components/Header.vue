<template>
  <header class="header-container">

<div class="top-bar">
      
      <img src="../assets/images/gym_logo_1x.png" alt="Logo" class="img-fluid logo-header">

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
      <p class="sub-title">Motivation is what gets you started. habit is what keeps you going.</p>
      <button class="btn btn-primary cta-header-button">JOIN US TODAY</button>
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



.header-container {
  display: flex;
  flex-direction: column;
background-image: url(../assets/images/home-banner.jpg);
background-position: center;
background-repeat: no-repeat;
background-size: cover;
  justify-content: space-between;
  padding: 20px;
  background-color: #333; 
  color: white;
  
}





.top-bar{
  display: flex;
  flex-direction: row;
  width: 100%;
  justify-content: space-between;
}

.navbar-nav {
  display: flex;
  flex-direction: row;
width: 60%;
  list-style: none;
  margin: 0;
  padding: 0;
  flex-wrap: nowrap;
}

.nav-item {
  margin-right: 15px;



}

.logo-header {
  width: 200px;
}
.nav-link {
  text-decoration: none;
  color: white;
 font-size: 10px;
 width: 100%;
 white-space: nowrap;
 
}

.nav-link:hover {
  text-decoration: none;
  color: rgb(180, 15, 15);
 font-size: 10px;
 width: 100%;
 white-space: nowrap;
 
}

.header-content {
  text-align: center;
  padding: 10rem;
  font-size: 30px;
}

.sub-title {
  font-size: 12px;
  margin-bottom: 30px;
}
.cta-header-button{
  background-color: rgba(240, 248, 255, 0);
  padding: 15px;
  color: rgba(255, 255, 255, 0.489);
  border-radius: 5px;
  border-color: rgba(255, 255, 255, 0.264);
}
</style>
