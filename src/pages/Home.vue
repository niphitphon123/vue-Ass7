<template>
 <div>
    <navbar />
    <section class="home">

<div class="image">
    <img src="images/profile.png" alt="">
</div>

<div class="content">
    <h3>{{Name}}</h3>
    <span>"Hello World"</span>
    <p>Hello, My Name Is Niphitphon Preedeesakulchai. My Nickname Is Pete. Now I'm 19 Years Old. Now I'm Studying Multimedia & Entertainment Engineering At Bangkok University. I graduated from Nawaminthrachinuthit Bodindecha school. My favourite sport is Basketball and Volleyball. And my hobby is playing game. </p>

</div>
<div class="content">
    <p> <span>name : </span> {{mrs}} </p>
    <p> <span>age : </span> {{age}} </p>
        <p> <span>email : </span> {{email}} </p>
            <p> <span>address : </span> 648 Chokchai4 Ladprao 10230 Bangkok </p>
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
            Name: 'Niphitphon Preedeesakulchai',
            motto: 'Hello World',
            mrs: 'Niphitphon Preedeesakulchai',
            age: '19',
            email: 'niphitphon.pree@bumail.net',
            address: '648 Chokchai4 Ladprao 10230 Bangkok'


        } 
    }


}
</script>

<style>

</style>