<template>
  <header class="cta-container">


    <div class="content-cta">
      <img src="../assets/images/home_img-compressor-400x222.jpg" alt="xx">


      <div class="cta-input">
      <p class="sub-title-slogan">Sign Up For A Free Training Session!</p>
   
    <label for="name">Name </label>
    <input v-model="name" type="text" id="name" required />

    <label for="email">Email</label>
    <input v-model="email" type="email" id="email" />

    <button @click="startNow" class="btn btn-danger button-cta">Start Now!</button>
  </div>
  <div>
    </div>
    </div>






  </header>
</template>

<script>
export default {
  data() {
    return {
      name: '',
      email: '',
    };
  },
  methods: {
    startNow() {
      // Azioni da eseguire quando il pulsante viene premuto
      console.log('Start Now!', this.name, this.email);
      // Puoi eseguire altre azioni, ad esempio l'invio di dati a un server
    },
  },
};


</script>

<style>



.cta-container {
  display: flex;
  flex-direction: row;
width: 100%;
  justify-content: center;
  background-color: rgb(37, 37, 37); 
  color: white;
  
}

.text-center-slogan {
  font-size: 25px;
}

.cta-input{
  display: flex;
  flex-direction: column;
  margin-left: 50px;
  width: 40%;


}

.content-cta {
  display: flex;
  flex-direction: row;
  text-align: center;
  padding: 5rem;
  font-size: 10px;
  color: rgba(255, 255, 255, 0.472);
  width: 100%;
 text-align: start;
 justify-content: center;



  
}

input {
  background-color: transparent; /* Background trasparente */
  border-radius: 5px;
  border: 1px solid rgba(255, 255, 255, 0.483); /* Linea inferiore bianca */
  color: rgba(255, 255, 255, 0.487);
  margin-bottom: 10px;
  padding: 5px;
  margin-top: 5px;
  outline: none; /* Rimuove la sottolineatura al focus */
}

input::placeholder {
  color: rgba(255, 255, 255, 0.8); /* Colore del testo del placeholder */
}
.sub-title-slogan {
  font-size: 12px;
  margin-bottom: 30px;
  color: rgba(255, 255, 255, 0.552);
  width: 100%;
}

.button-cta{
  background-color: rgb(247, 90, 90);
  border-style: none;
  padding: 10px;
  color: white;
  text-transform: uppercase;
  margin-top: 20px;
}
</style>
