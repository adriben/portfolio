<template>
    <div class="contact">
        <div class="contact-el">
<i class="fas fa-envelope-open-text gmail"></i>
<p>adrbenete@gmail.com</p>
        </div>
<div class="contact-el">
    <a href="https://www.linkedin.com/in/adrien-b%C3%A9n%C3%A9t%C3%A9-479b54217/">
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
<i class="fab fa-instagram-square"></i>
<p>Follow me on instagram</p>
</a>
</div>

<div class="contact-el">
<i class="fab fa-line"></i>


<p>aduBen</p>
</div>












    </div>
</template>

<script>


export default {
    name: 'Contact',
}
</script>

<style lang='scss'>
.contact{
    display: flex;
    align-content: center;
    justify-content: center;
    .contact-el{
        margin: 2rem;
        font-size: 130%;
        a{
            text-decoration: none;
            color: black;
    
        }
        i{
            font-size: 200%;
            transition: 500ms;
            &:hover{
                transform: scale(1.3);
                transition: 500ms;
            }
        }
    }
    .gmail{
        color: rgb(218, 56, 56);
    }
    .fa-linkedin{
        color: rgb(25, 25, 175);
    }
    .fa-line{
        color: rgba(36, 201, 36, 0.808);
    }
    .fa-instagram-square{
       font-size: 40px;      
        color: rgb(165, 24, 165);
      
      
    }
}

</style>