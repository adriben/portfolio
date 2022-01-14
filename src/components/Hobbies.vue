<template>
  <div class="hobbies">
    <div class="hobbies-el">
      <i class="fas fa-chess" data-aos="zoom-in"></i>
      <p>Chess</p>
    </div>
    <div class="hobbies-el">
      <i class="fas fa-bicycle" data-aos="zoom-in"></i>
      <p>Cycling</p>
    </div>

    <div class="hobbies-el">
      <i class="fas fa-camera-retro" data-aos="zoom-in"></i>
      <p>Photography</p>
    </div>

    <div class="hobbies-el">
      <i class="fas fa-film" data-aos="zoom-in"></i>
      <p>Cinema</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Hobbies",
};
</script>

<style lang="scss">
.hobbies {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  align-content: center;
  justify-content: center;
  @media screen and (max-width: 970px) {
    grid-template-columns: 1fr 1fr;
  }
  @media screen and (max-width: 500px) {
    grid-template-columns: 1fr;
  }
  .hobbies-el {
    margin: 1rem;
    font-size: 130%;
    i {
      font-size: 170%;
    }
  }
}
</style>
