<template>
  <div class="landing">
    <nav>
     <p class="logo">sunnyside</p>
    <div class="links">
      <router-link style="text-decoration: none; color: inherit;padding:20px;" to="/about">About</router-link>
      <router-link style="text-decoration: none; color: inherit;padding:20px;" to="/services">Services</router-link>
      <router-link style="text-decoration: none; color: inherit;padding:20px;" to="/">projects</router-link> 
     
    
    <router-link style="text-decoration: none; color: black;background-color:white;border-radius:2rem;width:150px; padding:20px;text-align:center" to="/services">CONTACT</router-link>
    </div>
  </nav>
  <router-view/>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@600&family=Fraunces:ital,wght@1,700&display=swap');

nav{
  font-family: 'Barlow', sans-serif;
  display: flex;
  justify-content: space-between;
  padding: 30px;
  color: hsl(0, 0%, 100%);
}
.links{
  font-size: 1.2rem;
  width: 600px;
  display: flex;
  justify-content: space-around;
  font-weight: lighter;
}
.landing{
  background: url("../public/image-header.jpg");
  height: 100vh;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.logo{
  font-size: 2.3rem;
  font-family: 'Barlow', sans-serif;
  font-weight: 900;  
}
</style>
