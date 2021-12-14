<template>
  <div class="home">
     <TheHeader></TheHeader>
   <img src="..\assets\coding-vs-programming-2.jpg" alt="picture of a web developer">
   <div class="container">
     <h2>About me</h2>
     <p class="pb-5">Inspired by the creative aspect of Web Developing, I recently completed an online program with Openclassrooms. 
       I am mainly focused on frontend but I also acquired some skills in backend developement with Node Js. 
       I am really motivated and eager to learn, and most of all I enjoy coding</p>
       <h2 class="text-center pb-3">My Skills</h2>
       <img src="../assets/html.png" alt="logo html" class="logo">
       <img src="../assets/css.png" alt="logo css" class="logo css">
       <img src="../assets/js.png" alt="logo javascript" class="logo">
       <img src="../assets/logo.png" alt="logo vue" class="logo">
       <img src="../assets/sass.png" alt="logo sass" class="logo">
       <img src="../assets/bootstrap.png" alt="logo bootstrap" class="logo">
       <img src="../assets/mysql.png" alt="logo mysql" class="logo">
       <img src="../assets/mongo.png" alt="logo mongodb" class="logo">
       <img src="../assets/node.png" alt="logo node" class="logo">
       

       
   </div>
   <br>
   <h2 class="text-center pt-4">My works</h2>
   <br>
   <div class="row">

     
     <div class="card mb-5">
  <img class="card-img-top reservia" src="..\assets\reservia.png" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Reservia</h5>
    <p class="card-text">Turn Mock-ups Into a Web Page with HTML & CSS,  implementing a travel booking platform's website from scratch. The page is responsive</p>
    <div class="pb-3">
       
    <img src="../assets/html.png" alt="logo html" class="logo">
    <img src="../assets/css.png" alt="logo css" class="logo css">

    </div>
   
    <a href="#" class="btn btn-primary mr-5">Check the webpage</a>
    <a href="#" class="btn btn-secondary ml-3">Check the code</a>
    <img class="iphone" src="../assets/iphone.png" alt="iphone picture" id="reservia">
    
  </div>
</div>
<div class="card mb-5">
  <img class="card-img-top ohmyfood" src="..\assets\ohmyfood.png" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Ohmyfood</h5>
    <p class="card-text">Integrate a mobile website with animations in CSS. Implement the mobile version of this foodtech website with CSS animations.</p>
    <div class="pb-3">
       
    <img src="../assets/html.png" alt="logo html" class="logo">
    <img src="../assets/css.png" alt="logo css" class="logo css">
    <img src="../assets/sass.png" alt="logo sass" class="logo">

    </div>
    <a href="#" class="btn btn-primary mr-5">Check the webpage</a>
    <a href="#" class="btn btn-secondary ml-3">Check the code</a>
    <img class="iphone" src="../assets/iphone.png" alt="iphone picture" id="ohmyfood">
    
    
  </div>
</div>
<div class="card mb-5">
  <img class="card-img-top" src="..\assets\coding-vs-programming-2.jpg" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Optimize an Existing Website (La Chouette agence)</h5>
    <p class="card-text">Research and implement current best practices and standards in web development, including SEO, size and speed, and accessibility.</p>
    <div class="pb-3">
       
    <img src="../assets/seo.png" alt="logo seo" class="logo">
    <img src="../assets/analytics.png" alt="logo analytics" class="logo analytics">

    </div>
    <a href="#" class="btn btn-primary">Go somewhere</a>
    
    
  </div>
</div>
<div class="card mb-5">
  <img class="card-img-top" src="..\assets\coding-vs-programming-2.jpg" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Optimize an Existing Website (La Chouette agence)</h5>
    <p class="card-text">Research and implement current best practices and standards in web development, including SEO, size and speed, and accessibility.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
    
    
  </div>
</div>



   </div>
   <footer>
     Footer
   </footer>
   
  </div>
</template>

<script>
// @ is an alias to /src
import TheHeader from '@/components/TheHeader.vue'

export default {
  name: 'Home',
  components: {
    "TheHeader": TheHeader
  }
}
</script>
<style lang="scss">

img{
  width: 100%;
  margin: auto;
  max-width: 1700px;
  object-fit: cover;
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
  width: 60px
}

.card{
  width: 40rem;
  position: relative;
  border: solid 1px rgba(128, 128, 128, 0.678);
  z-index: 1;
  border-radius: 5px;

  
  .card-img-top {
    height: 30rem;
    object-fit: cover;
    
  }
  .logo{
  width: 60px;
  padding-right: 1rem;
  transition: 100ms;
  }
  .css{
    width: 50px;
  }
  .analytics{
    width: 7rem;
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
      top: 270px;
      right: 20px;
      background-size: 8rem;
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


</style>