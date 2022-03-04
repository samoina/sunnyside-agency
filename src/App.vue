<template>
  <div class="landing">
    <nav>
     <p class="logo">sunnyside</p>
    <div class="links">
      <router-link style="text-decoration: none; color: inherit;padding:20px;" to="/">About</router-link>
      <router-link style="text-decoration: none; color: inherit;padding:20px;" to="/services">Services</router-link>
      <router-link style="text-decoration: none; color: inherit;padding:20px;" to="/">projects</router-link>      
    
    <router-link style="text-decoration: none; color: black;background-color:white;border-radius:2rem;width:150px; padding:20px;text-align:center" to="/services">CONTACT</router-link>
    </div>
  </nav>
  <router-view/>
  </div>
  <section class="cards">
    <div class="card-text-section">
      <div class="text-section">
        <p class="text-section-heading">Transform your brand</p>
      <p class="text">We are a full-service creative agency specializing in helping brands grow fast. Engage your clients through compelling visuals that do most of the marketing for you.</p>
      <a href="#" class="learn-link">LEARN MORE</a>
      </div>
      </div>
      <div class="about-image">
        </div>     
  </section>
  <section class="cards">
    <div class="standout-image">
        </div>
    <div class="card-text-section">
      <div class="text-section">
        <p class="text-section-heading">Stand out to the right audience</p>
      <p class="text">Using a collaborative formula of designers, reserchers, photographers, videographers, and copyrighters we'll build abd extend your brand in digital places.</p>
      <a href="#" class="learn-link standout">LEARN MORE</a>
      </div>
      </div>
      
  </section>
  <section class="cards">
    <div class="graphic-design">
      <div class="services-section">
         <p class="services-header">Graphic design</p>
         <p class="services-text">Great design makes you memorable. We deliver artwork that underscores your brand message and captures potential clients' attention</p>
      </div>
    </div>
    <div class="photography">
      <div class="services-section">
         <p class="services-header">Photography</p>
         <p class="services-text">Increase your credibilty by getting the most stunning high-quality photos that improve your business image</p>
      </div>
    </div>
  </section>

  <section class="testimonials">
     <div class="testimonial-card">
       <p class="testimonial-header">CLIENT TESTIMONIALS</p>
      <div class="testimonial-cards">
         <div class="test-cards">
           <img class="user-img" src="../public/images/image-emily.jpg"/>
           <p class="test-text">We put our trust in sunnyside and they delivered, making sure our needs were met and deadlines were always hit</p>
           <div class="test-footer">
              <p class="name">Emily R.</p>
              <p class="occupation">Marketing Director</p>
           </div>
         </div>
         <div class="test-cards">
           <img class="user-img" src="../public/images/image-thomas.jpg"/>
           <p class="test-text">
             Sunnyside's enthusiasm coupled with their keen interest in our brand's success made it a satisfying and enjoyable experience.
           </p>
           <div class="test-footer">
              <p class="name">Thomas S.</p>
              <p class="occupation">Chief Operating Officer</p>
           </div>
         </div>
         <div class="test-cards">
           <img class="user-img" src="../public/images/image-jennie.jpg"/>
           <p class="test-text">
             Incredible end result! Our sales increased over 400% when we worked with Sunnyside.Highly recommended
           </p>
           <div class="test-footer">
              <p class="name">Jennie F.</p>
              <p class="occupation">Business Owner</p>
           </div>
         </div>
      </div>
     </div>
  </section>
  <section class="gallery">
    <div class="gallery-images one">
      <!-- <img class="gallery-img" src="../public/image-gallery-milkbottles.jpg"/> -->

    </div>
    <div class="gallery-images two">
      <!-- <img class="gallery-img" src="../public/image-gallery-orange.jpg"/> -->
    </div>
    <div class="gallery-images three">
      <!-- <img class="gallery-img" src="../public/image-gallery-cone.jpg"/> -->
    </div>
    <div class="gallery-images four">
      <!-- <img class="gallery-img" src="../public/image-gallery-sugarcubes.jpg"/> -->
    </div>
  </section>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@600&family=Fraunces:wght@800&display=swap');

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
.cards{
  height: 80vh;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}
.card-text-section{
  display: flex;
  justify-content: center;
  align-items: center;
}
.text-section{
  width: 55%;
  height: 50%;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
}
.text-section-heading{
  font-family: 'Fraunces', serif;
  font-size: 2.9rem;
}
.text{
  font-size: 20px;
  text-align: justify;
  color:hsl(232, 10%, 55%);
}
.learn-link{
  text-decoration: none;
   color: black;
   position: relative;
  font-family: 'Fraunces', serif;
  width:fit-content;
  border-bottom: 4px solid hsl(51, 100%, 49%);
}
.standout{
   border-bottom: 4px solid  hsl(7, 99%, 70%);
}
.about-image, .standout-image, .graphic-design, .photography{
  background-position: center;
  background-repeat: no-repeat;
  background-size:cover;
}
.about-image{
  background-image: url("../public/image-transform.jpg");
}
.standout-image{
   background-image: url("../public/image-stand-out.jpg");
}
.graphic-design, .photography{
  display: flex;
  align-items: flex-end;
  justify-content: center;
  padding: 30px;
  font-weight: bold;
}
.graphic-design{
  background-image: url("../public/image-graphic-design.jpg");
  color: hsl(167, 40%, 24%);
}
.photography{
  background-image: url("../public/image-photography.jpg");
  color: hsl(198, 62%, 26%);
}
.services-section{
  display: flex;
  flex-direction: column;
  height: 200px;
  text-align: center;
  justify-content: space-around; 
}
.services-header{
  font-family: 'Fraunces', serif;
  font-size: 2rem;
}
.services-text{
  font-size: 20px;
  text-align: center;
  width: 50%;
  align-self: center;
}
.testimonials{
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
.testimonial-card{
  height: 60vh;
  width: 70vw;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.testimonial-header{
  font-size: 2rem;
  text-align: center;
  color: hsl(213, 9%, 39%);
  font-family: 'Fraunces', serif;
}
.testimonial-cards{
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  column-gap: 50px;
  height:500px;
}
.test-cards{
  height: 80%;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: center;
}
.user-img, .gallery-img{
  object-fit: contain;
}
.user-img{
  height: 80px;
  width: 80px;
  border-radius: 2.5rem;
}
.test-text{
  text-align: center;
  font-size: 18px;
  font-family: 'Barlow', sans-serif;
  color: hsl(213, 9%, 39%);  
}
.name{
  font-family: 'Fraunces', serif;
  font-size: 1.2rem;
}
.occupation{
   color: hsl(213, 9%, 39%); 
}
.test-footer{
line-height: 40px;
}
.gallery{
  display: grid;
  grid-template-columns: repeat(4,1fr);
  height: 60vh;
}
.one{
  background: url("../public/image-gallery-milkbottles.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.two{
  background: url("../public/image-gallery-orange.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.three{
  background: url("../public/image-gallery-cone.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.four{
  background: url("../public/image-gallery-sugarcubes.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
