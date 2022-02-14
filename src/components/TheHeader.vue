<template>
  <header class="bg-dark">
    <div class="">
      <div>
        <nav class="navbar navbar-expand-lg navbar-dark">
          <p class="navbar-brand" v-if="eng">
            <i class="fas fa-laptop"></i>
            Web developer in Fukuoka
          </p>
          <p class="navbar-brand" v-else>
            <i class="fas fa-laptop"></i>
            福岡のWebデベロッパー
          </p>
          <button
            class="navbar-toggler"
            type="button"
            data-toggle="collapse"
            data-target="#navbarContent"
            aria-controls="navbarContent"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div id="navbarContent" class="collapse navbar-collapse">
            <ul class="navbar-nav">
              <li class="nav-item active">
                <a class="nav-link" href="#aboutMe" v-if="eng"
                  ><i class="fas fa-address-card"></i> About Me</a
                >
                <a class="nav-link" href="#aboutMe" v-else
                  ><i class="fas fa-address-card"></i> 私について</a
                >
              </li>
              <li class="nav-item text-right active">
                <a class="nav-link" href="#myWorks" v-if="eng"
                  ><i class="fas fa-palette"></i> My works</a
                >
                <a class="nav-link" href="#myWorks" v-else
                  ><i class="fas fa-palette"></i> プロジェクト</a
                >
              </li>
              <li class="nav-item text-right active">
                <a class="nav-link" href="#contact" v-if="eng"
                  ><i class="fas fa-phone"></i> Contact</a
                >
                <a class="nav-link" href="#contact" v-else
                  ><i class="fas fa-phone"></i> 連絡先</a
                >
              </li>
              <li class="nav-item text-right active pl-5">
                <a class="nav-link" href="" @click="changeLang" v-if="eng"
                  ><img
                    src="../assets/japan.png"
                    alt="japanese flag"
                    class="flag"
                  />日本語
                </a>
                <a class="nav-link" href="" @click="changeLang" v-else
                  ><img
                    src="../assets/english.png"
                    alt="japanese flag"
                    class="flag"
                  />English
                </a>
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
  name: "TheHeader",
  data() {
    return {
      eng: true,
    };
  },
  methods: {
    changeLang(e) {
      this.eng = !this.eng;
      e.preventDefault();
      this.$parent.changeLang();
    },
  },
};
</script>

<style lang="scss">
header {
  font-size: 130%;
  position: fixed;
  z-index: 4;
  width: 100%;

  a {
    color: #ffff;
    padding-left: 1rem;
    transition: 400ms;
    &:hover {
      transform: scale(1.15);
      transition: 400ms;
    }
  }
  ul {
    margin-right: 0;
  }
  li {
    padding-left: 2rem;
  }
  .navbar-expand-lg .navbar-collapse {
    justify-content: flex-end;
  }
}
.flag {
  width: 2rem;
}
</style>
