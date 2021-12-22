<template>
     <header class="bg-dark ">
        <div class="">
          <div>
            <nav class="navbar navbar-expand-lg navbar-dark">
              <p class="navbar-brand">
                <i class="fas fa-laptop"></i>
                Web developer in Fukuoka
              </p>
              <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarContent" aria-controls="navbarContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
              </button>
              <div id="navbarContent" class="collapse navbar-collapse">
                <ul class="navbar-nav">
                  <li class="nav-item active">
                      
                    <a class="nav-link" href="#aboutMe"><i class="fas fa-address-card"></i> About Me</a>
                  </li>
                  <li class="nav-item text-right active">
                      
                    <a class="nav-link" href="#myWorks"><i class="fas fa-palette"></i> My works</a>
                  </li>
                  <li class="nav-item text-right active">
                      
                    <a class="nav-link" href="#contact"><i class="fas fa-phone"></i> Contact</a>
                  </li>
                  <li class="nav-item text-right active pl-5">
                      
                    <a class="nav-link" href="">日本語 </a>
                  </li>
                  
                </ul>
              </div>
            </nav>
          </div>
        </div>    
    </header>
</template>

<script>


export default {
    name: 'TheHeader',
}
</script>

<style lang="scss">
header {
    font-size: 130%;
    position: fixed;
    z-index: 4;
    width: 100%;
    
   
    a{

    color: #ffff;
    padding-left: 1rem;
    transition: 400ms;
    &:hover{
    transform: scale(1.15);
    transition: 400ms;
  }
  
   }
   ul{
     margin-right: 0;
   }
   li{
      padding-left: 2rem;
   }
  .navbar-expand-lg .navbar-collapse{
    justify-content: flex-end;
  }  
}
</style>