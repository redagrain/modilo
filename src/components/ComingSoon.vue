
<template>
  <div class="hero">
    <div class="blur"></div>
    <div class="content">
      <div class="logo">
        <img src="../assets/logo-transparent.png" alt="logo"/>
      </div>
      <img class="spinner" src="../assets/spinner.svg" alt="">
      <h1>Coming Soon</h1>
      <p>Get ready to discover your new favorite outfits!</p>
    </div>
  </div>
</template>

<style scoped>
.hero {
  position: relative;
  height: 100vh;
  width: 100vw;
  background-color: #0f044d;
  display: flex;
  align-items: center;
  justify-content: center;
}

.content{
  width: 90%;
  height: 90%;
  margin: auto;
  border-radius: 10px;
  background: url('/src/assets/hoodie.png') center/contain no-repeat ;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  color: #fff;
  font-family: Arial, Helvetica, sans-serif;
  gap: 20px;
}

.logo{
  width: 150px;
  height: 150px;
}

.logo img{
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.content h1{
  text-transform: uppercase;
}

.spinner{
  width: 50px;
  animation: spin 2s infinite ;
}

@keyframes spin {
  from {
    transform: rotate(0deg) scale(0.9);
  }
  to {
    transform: rotate(360deg) scale(1.05);
  }
}
.blur{
  width: 200px;
  height: 300px;
  border-radius: 999px;
  background-color: #F44336;
  position: absolute;
  left: -30px;
  filter: blur(100px);
  opacity: 0.9;
  top:-50px;
}

</style>
