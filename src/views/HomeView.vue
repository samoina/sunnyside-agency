
<template>
  <div class="home">
  <p class="tagline">WE ARE CREATIVES</p>
   <img src="../../public/images/icon-arrow-down.svg" class="down-arrow"/>
  </div>
</template>

<script>
// @ is an alias to /src
export default {
  name: 'HomeView',
  
}
</script>

<style scoped>
.home{
  display: flex;
  flex-direction: column;
  height: 450px;
  margin-top:40px;
  justify-content: space-around;
  align-items: center;
}
   .tagline{
     color:hsl(0, 0%, 100%);
     font-size:4rem;     
     font-weight: 900;
     letter-spacing: 3px;
   }
   .down-arrow{
     height: 150px;
   }
</style>
