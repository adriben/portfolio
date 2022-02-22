<template>
  <div class="contact">
    <div class="contact-el">
      <i class="fas fa-envelope-open-text gmail"></i>
      <p>adrbenete@gmail.com</p>
    </div>
    <div class="contact-el">
      <a
        href="https://www.linkedin.com/in/adrien-b%C3%A9n%C3%A9t%C3%A9-479b54217/"
      >
        <i class="fab fa-linkedin"></i>

        <p>My linkedin profile</p>
      </a>
    </div>

    <div class="contact-el">
      <a href="https://github.com/adriben">
        <i class="fab fa-github"></i>
        <p>My github page</p>
      </a>
    </div>

    <div class="contact-el">
      <a href="https://www.instagram.com/adribenete/">
        <img src="../assets/insta.png" alt="logo instagram" class="insta" />
        <p>Follow me on instagram</p>
      </a>
    </div>

    <div class="contact-el">
      <i class="fab fa-line"></i>

      <p>aduben</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contact",
};
</script>

<style lang="scss">
.contact {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
  @media screen and (max-width: 970px) {
    grid-template-columns: 1fr;
  }

  align-content: center;
  justify-content: center;
  .contact-el {
    margin: 2rem;
    font-size: 130%;
    a {
      text-decoration: none;
      color: white;
    }
    i {
      font-size: 200%;
      transition: 500ms;
      &:hover {
        transform: scale(1.3);
        transition: 500ms;
      }
    }
  }
  .gmail {
    color: rgb(218, 56, 56);
  }
  .fa-linkedin {
    color: rgb(17, 102, 238);
  }
  .fa-line {
    color: rgba(36, 201, 36, 0.808);
  }
  .insta {
    width: 40px;
    margin-top: 0.25rem;
    &:hover {
      transform: scale(1.3);
      transition: 500ms;
    }
  }
}
</style>
