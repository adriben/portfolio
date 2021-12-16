<template>
  <div class="home">
     <TheHeader class="mb-4"></TheHeader>
     <section class="banniere col-12 hero">
        <div class="hero-text">
          <p>Hi, my name is Adrien</p>
    
          <h1 class="pt-4 text-center">
          I am a Web developer
            <br>
            <span class="typed-text">{{ typeValue }}</span>
            <span class="cursor" :class="{'typing': typeStatus }">&nbsp;</span>
           </h1>
        </div>
      </section>
      <img src="../assets/id.png" alt="id picture" class="id-pic" data-aos="zoom-in" data-aos-duration="1800">
   <div class="container" id="aboutMe">
     <h2  class="mt-5 pt-2 text-center">About me</h2>
     <p class="aboutMePar">Inspired by the creative aspect of Web Developing, I recently completed an online program with Openclassrooms. 
       I am mainly focused on frontend but I also acquired some skills in backend developement with Node Js. 
       I am really motivated and eager to learn, and most of all I enjoy coding</p>
       <div class="text-center mb-5 pb-3">
        <a href="#" class="btn btn-secondary text-center"><i class="fas fa-download"></i> Download my resume in PDF</a>
       </div>
       
       <h2 class="text-center pb-3">My Skills</h2>
       <div class="text-center">
       <img src="../assets/html.png" alt="logo html" class="logo htmlD" data-aos="zoom-in-up" data-aos-duration="2400">
       <img src="../assets/css.png" alt="logo css" class="logo css cssD" data-aos="zoom-in-up" data-aos-duration="2000">
       <img src="../assets/js.png" alt="logo javascript" class="logo js jsD" data-aos="zoom-in-up" data-aos-duration="1800">
       <img src="../assets/logo.png" alt="logo vue" class="logo vue vueD" data-aos="zoom-in-up" data-aos-duration="1600">
       <img src="../assets/sass.png" alt="logo sass" class="logo sassD" data-aos="zoom-in-up" data-aos-duration="1400">
       <img src="../assets/bootstrap.png" alt="logo bootstrap" class="logo bootstrapD" data-aos="zoom-in-up" data-aos-duration="1200">
       <img src="../assets/mysql.png" alt="logo mysql" class="logo mysql mysqlD" data-aos="zoom-in-up" data-aos-duration="1000">
       <img src="../assets/mongo.png" alt="logo mongodb" class="logo mongo mongoD" data-aos="zoom-in-up" data-aos-duration="800">
       <img src="../assets/node.png" alt="logo node" class="logo node nodeD" data-aos="zoom-in-up" data-aos-duration="600">
       <img src="../assets/lr.png" alt="logo lr" class="logo lr lrD" data-aos="zoom-in-up" data-aos-duration="400">
       </div>
      

       
   </div>
   <br>
   <h2 class="text-center pt-4 mb-5">My works</h2>
   <br>
   <div class="row">

     
     <div class="card mb-5">
  <img class="card-img-top reservia" src="..\assets\reservia.png" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Reservia</h5>
    <p class="card-text">Turn Mock-ups Into a Web Page with HTML & CSS,  implementing a travel booking platform's website from scratch. The page is responsive</p>
    <div class="pb-3">
       
    <img src="../assets/html.png" alt="logo html" class="logo" data-aos="fade-right">
    <img src="../assets/css.png" alt="logo css" class="logo css" data-aos="fade-right">

    </div>
   
    <a href="https://adriben.github.io/AdrienBenete_2_27072021/" class="btn btn-primary">Check the webpage</a>
    <a href="https://github.com/adriben/AdrienBenete_2_27072021" class="btn btn-secondary ml-3">Check the code</a>
    <img class="iphone" src="../assets/iphone.png" alt="iphone picture" id="reservia">
    
  </div>
</div>
<div class="card mb-5">
  <img class="card-img-top ohmyfood" src="..\assets\ohmyfood.png" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Ohmyfood</h5>
    <p class="card-text">Integrate a mobile website with animations in CSS. Implement the mobile version of this foodtech website with CSS animations.</p>
    <div class="pb-3">
       
    <img src="../assets/html.png" alt="logo html" class="logo" data-aos="fade-right">
    <img src="../assets/css.png" alt="logo css" class="logo css" data-aos="fade-right">
    <img src="../assets/sass.png" alt="logo sass" class="logo" data-aos="fade-right">

    </div>
    <a href="https://adriben.github.io/AdrienBenete_3_15082021/" class="btn btn-primary">Check the webpage</a>
    <a href="https://github.com/adriben/AdrienBenete_3_15082021"  class="btn btn-secondary ml-3">Check the code</a>
    <img class="iphone" src="../assets/iphone.png" alt="iphone picture" id="ohmyfood">
    
    
  </div>
</div>
<div class="card mb-5">
  <img class="card-img-top" src="..\assets\lachouetteagence.png" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Optimize an Existing Website (La Chouette agence)</h5>
    <p class="card-text">Research and implement current best practices and standards in web development, including SEO, size and speed, and accessibility.</p>
    <div class="pb-3">
       
    <img src="../assets/seo.png" alt="logo seo" class="logo" data-aos="fade-right">
    <img src="../assets/analytics.png" alt="logo analytics" class="logo analytics" data-aos="fade-right">

    </div>
    <a href="https://github.com/adriben/AdrienBenete_4_27082021" class="btn btn-primary">Code after optimization</a>
    <a href="https://github.com/adriben/chouetteAgenceBEFORE" class="btn btn-secondary ml-3">Code before optimization</a>
    <img class="performance" src="../assets/performance.png" alt="iphone picture" id="performance">
    
    
    
  </div>
</div>
<div class="card mb-5">
  <img class="card-img-top" src="..\assets\orinocamera.png" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Build an e-commerce Website with JavaScript</h5>
    <p class="card-text">Created the desing and use an API to collect information about products and add a cart feature for purchases. Utilisation of fetch, localstorage, I did all the front end part. It allowed me to learn and improve myself in vanilla javascript (no framework)</p>
    <div class="pb-3">
       
    <img src="../assets/html.png" alt="logo html" class="logo" data-aos="fade-right">
       <img src="../assets/css.png" alt="logo css" class="logo css" data-aos="fade-right">
       <img src="../assets/sass.png" alt="logo sass" class="logo" data-aos="fade-right">
       <img src="../assets/bootstrap.png" alt="logo bootstrap" class="logo" data-aos="fade-right">
       <img src="../assets/js.png" alt="logo javascript" class="logo" data-aos="fade-right">
       <img src="../assets/ux.png" alt="logo design" class="logo ux" data-aos="fade-right">

    </div>
    <a href="#" class="btn btn-primary mr-3">Check the video Demo</a>
    <a href="https://github.com/adriben/AdrienBenete_5_27092021/tree/main/frontend" class="btn btn-secondary">Check the code</a>
    
    
  </div>
</div>

<div class="card mb-5">
  <img class="card-img-top" src="..\assets\hotsauce.png" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Build a Secure API for a Review App</h5>
    <p class="card-text">Build the back end for a new app, Hot Takes, where customers review specialty hot sauces. Use Node.js, Express, and MongoDB to build its NoSQL database. Secure customer data by applying the OWASP web security standards.</p>
    <div class="pb-3">
       
    <img src="../assets/node.png" alt="logo node" class="logo node" data-aos="fade-right">
    <img src="../assets/mongo.png" alt="logo mongo" class="logo mongo" data-aos="fade-right">
    

    </div>
    <a href="#" class="btn btn-primary">Check the video Demo</a>
    <a href="https://github.com/adriben/AdrienBenete_6_26102021/tree/main/backend" class="btn btn-secondary ml-3">Check the code</a>

    
    
    
  </div>
</div>

<div class="card mb-5">
  <img class="card-img-top" src="..\assets\groupomania.png" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Build a Full-Stack Corporate Social Network </h5>
    <p class="card-text">Analyze a client’s needs to define the scope and features of a new application. With the help of a front-end framework (Vue.js), build a full-stack solution, including a SQL database. The user is able to share a post, like and comment.</p>
    <div class="pb-3">
       
    <img src="../assets/logo.png" alt="logo vue" class="logo" data-aos="fade-right">
    <img src="../assets/vuex.png" alt="logo vue" class="logo" data-aos="fade-right">
    <img src="../assets/mysql.png" alt="logo mysql" class="logo" data-aos="fade-right">
    <img src="../assets/node.png" alt="logo node" class="logo node" data-aos="fade-right">
    <img src="../assets/ux.png" alt="logo design" class="logo ux " data-aos="fade-right">
    

    </div>
    <a href="#" class="btn btn-primary">Check the video Demo</a>
    <a href="https://github.com/adriben/AdrienBenete_7_19112021-" class="btn btn-secondary ml-3">Check the code</a>

    
    
    
  </div>
</div>



   </div>
   <div class="text-center">
     <h2>Contact</h2>
     <Contact></Contact>

   </div>
   <div class="text-center">
    <h3>Hobbies</h3>
   <Hobbies class="container"></Hobbies>
   </div>
   
   <footer>
     Footer
   </footer>
   
  </div>
</template>

<script>
// @ is an alias to /src

import TheHeader from '@/components/TheHeader.vue';
import Hobbies from '@/components/Hobbies.vue';
import Contact from '@/components/Contact.vue'
import AOS from 'aos';
import 'aos/dist/aos.css';





export default {
  name: 'Home',
  components: {
    "TheHeader": TheHeader,
    "Hobbies": Hobbies,
    "Contact": Contact
  },
  data:() =>{
    return{
      typeValue: '',
      typeStatus: false,
      typeArray: ['Front end', 'Full stack', 'Design'],
      typingSpeed: 200,
      erasingSpeed: 100,
      newTextDelay: 1500,
      typeArrayIndex: 0,
      charIndex: 0

    }
  },
  methods: {
    typeText(){
     if(this.charIndex < this.typeArray[this.typeArrayIndex].length){
           if(!this.typeStatus)
           this.typeStatus = true;
           this.typeValue += this.typeArray[this.typeArrayIndex].charAt(this.charIndex)
           this.charIndex += 1;

           setTimeout(this.typeText, this.typingSpeed);
     } else{
              this.typeStatus = false;
              setTimeout(this.eraseText, this.newTextDelay);
     }
    },
    eraseText(){
      if(this.charIndex > 0){
        if(!this.typeStatus)
        this.typeStatus = true;

        this.typeValue = this.typeArray[this.typeArrayIndex].substring(0, this.charIndex -1 )
        this.charIndex -= 1;
        setTimeout(this.eraseText, this.erasingSpeed)
      }
      else{
        this.typeStatus = false;
        this.typeArrayIndex += 1;
        if(this.typeArrayIndex >= this.typeArray.length)
        this.typeArrayIndex = 0;

        setTimeout(this.typeText, this.typingSpeed + 1000);
      }
    }
  },
  created(){
    setTimeout(this.typeText, this.newTextDelay + 200);
    AOS.init()
  }
}
</script>
<style lang="scss">
.home{
  background-color: rgba(255, 255, 255, 0.685);
  h2{
    color: #294446;
  }
}

img{
  width: 100%;
  
  margin: auto;
  max-width: 1700px;
  object-fit: cover;
}

.hero{
  
    color: white;
    background-image:linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url("../assets/shutterstock_1122339353.jpg");
    background-position: top;
    background-repeat: no-repeat;
    background-size: cover;
    height: 800px;
    width: 100%;
    position: relative;

    .hero-text{
        position: absolute;        
        align-items: center;
        top: 30%;
        left: 60%;
    p{
      position: absolute;
        font-size: 200%;
        top: -20%;
        left: 10%;
        animation: slideDisplay 3s;
        
      
    }
    h1{
      animation: slideDisplay 500ms;
      span.cursor{
        display: inline-block;
        margin-left: 3px;
        width: 4px;
        background-color: #fff;
        animation: cursorBlink 800ms infinite;
        
      }
      span.cursor.typing{
        animation: none;
        
      }
      span.typed-text{
       color: #E27D60;
      }

    }
    
    
  }}
.banner{
  height: 700px;
}
.id-pic{
  width: 8rem;
  height: 8rem;
 object-fit: cover;
  border-radius: 150px;
  position: absolute;
  left: 260px;
  top: 890px
}
.aboutMePar{
  font-size: 120%;
}
.logo{
  width: 80px;
  padding-right: 1rem;
  transition: 100ms;

  &:hover{
    transform: scale(1.3);
    transition: 300ms;
    cursor: pointer;

  }
}
.css{
  width: 60px;
  
}

.btn-secondary{
  background-color: #E27D60;
  
}


.card{
  width: 35rem;
  position: relative;
  z-index: 1;
  border-radius: 20px;
  box-shadow: 3px 3px 7px rgba(63, 62, 62, 0.596);
  transition: 400ms;
  &:hover{
    transform: scale(1.05);
    transition: 400ms;
  }

  
  .card-img-top {
    border-top-left-radius: 20px;
    border-top-right-radius: 20px;
    height: 29rem;
    object-fit: cover;
    border-bottom: 1px solid rgba(128, 128, 128, 0.308);
    
  }
  .logo{
  width: 60px;
  padding-right: 1rem;
  transition: 100ms;
  }
  .css{
    width: 50px;
  }
  .ux{
    width: 90px;
    position: absolute;
  }
  .analytics{
    width: 7rem;
  }
  .mongo{
    width: 9rem;
    padding-left: 1rem;
  }
  .node{

    width: 6rem;
  }
  .reservia{
      object-fit: cover;
      object-position: left top;
    }
    .ohmyfood{
    
     object-fit: cover;
     object-position: left top;
    
    }
    .iphone{
      height: 16rem;
      width: 7.6rem;
      position: absolute;
      top: 235px;
      right: 20px;
      background-size: 8rem;
      border-radius: 15px;
     box-shadow: 5px 3px 5px rgba(63, 62, 62, 0.596);
      z-index: 3;

    }
    .performance{
      height: 16rem;
      width: 25rem;
      position: absolute;
      top: 220px;
      right: -20px;
      background-size: 8rem;
      border: grey 1px solid;
      border-radius: 15px;
     box-shadow: 5px 3px 5px rgba(63, 62, 62, 0.596);
      z-index: 3;

    }
    #reservia{
      background-image: url("../assets/reserviaIphone1.png");
    }
    #ohmyfood{
    
      background-image: url("../assets/Menu.png");
      background-repeat: no-repeat;
    }
}

@keyframes cursorBlink{
  49%{ background-color: #fff;}
  50% {background-color: transparent;  }
  99% {background-color: transparent;  }

}
@keyframes slideDisplay{
  0%{
    transform: translateX(-100px);
    opacity: 0;

  }
  100%{
    transform: translateX(0);
    opacity: 1;
  }
}
@keyframes shake {
  10%, 90% {
    transform: translate3d(-1px, 0, 0);
  }
  
  20%, 80% {
    transform: translate3d(2px, 0, 0);
  }

  30%, 50%, 70% {
    transform: translate3d(-4px, 0, 0);
  }

  40%, 60% {
    transform: translate3d(4px, 0, 0);
  }
}

</style>