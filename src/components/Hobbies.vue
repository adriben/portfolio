<template>
    <div class="hobbies">
        <div class="hobbies-el">
<i class="fas fa-chess"></i>
<p>Chess</p>
        </div>
<div class="hobbies-el">
<i class="fas fa-bicycle"></i>
<p>Cycling</p>
</div>

<div class="hobbies-el">
    <i class="fas fa-camera-retro"></i>
    <p>Photographie</p>

</div>

<div class="hobbies-el">
<i class="fas fa-film"></i>
<p>Cinema</p>
</div>











    </div>
</template>

<script>


export default {
    name: 'Hobbies',
}
</script>

<style lang='scss'>
.hobbies{
    display: flex;
    align-content: center;
    justify-content: center;
    .hobbies-el{
        margin: 1rem;
        font-size: 130%;
        i{
            font-size: 170%;
        }
    }
}

</style>