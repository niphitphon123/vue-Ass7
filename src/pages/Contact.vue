<template>
 <div>
    <navbar />
    <section class="home">

<div class="image">
    <img src="images/profile123.png" alt="">
</div>
<div class="content">
            <p> <span>address : </span> 648 Chokchai4 Ladprao 10230 Bangkok </p>
                        </div>

<div class="content">
    <a href="https://www.facebook.com/savada.tsuna.1" class="btn"> Facebook <i class="fas fa-user"></i> </a>
    <a href="https://www.instagram.com/dt_pete/" class="btn"> Instagram <i class="fas fa-user"></i> </a>
    <a href="niphitphon.pree@bumail.net" class="btn"> Gmail <i class="fas fa-user"></i> </a>
    <a href="https://twitter.com/pete2003p" class="btn"> Twitter <i class="fas fa-user"></i> </a>
    <a href="/" class="btn"> 086-386-6384 <i class="fas fa-user"></i> </a>

</div>

</section>
 </div>
</template>

<script>
import Navbar from '../components/Navbar.vue';
export default {
    components: { Navbar } ,
    data() { 
        return { 
            address: '648 Chokchai4 Ladprao 10230 Bangkok'


        } 
    }


}
</script>

<style>

</style>