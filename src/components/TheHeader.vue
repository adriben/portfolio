<template>
     <header class="bg-dark">
        <div class="container">
          <div>
            <nav class="navbar navbar-expand-lg navbar-dark">
              <a class="navbar-brand" href="">
                <i class="fas fa-laptop"></i>
                Web developer in Fukuoka
              </a>
              <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarContent" aria-controls="navbarContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
              </button>
              <div id="navbarContent" class="collapse navbar-collapse">
                <ul class="navbar-nav">
                  <li class="nav-item active">
                      
                    <a class="nav-link" href="#aboutMe"><i class="fas fa-address-card"></i> About Me</a>
                  </li>
                  <li class="nav-item text-right active">
                      
                    <a class="nav-link" href=""><i class="fas fa-palette"></i> My works</a>
                  </li>
                  <li class="nav-item text-right active">
                      
                    <a class="nav-link" href=""><i class="fas fa-language"></i>日本語 </a>
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
   
    a{

    color: #ffff;
    padding-left: 1rem;
   }
   li{
      padding-left: 2rem;
   }
  .navbar-expand-lg .navbar-collapse{
      padding-left: 15rem;
    justify-content: flex-end;
  }  
}
</style>