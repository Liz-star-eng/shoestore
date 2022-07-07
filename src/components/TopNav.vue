<template>
<body>
<nav class="TopMostNav">
    <div class="contact">
        <a href=""><i class="fa fa-envelope-o"> jcsnkrs800@gmail.com</i></a>
        <a href=""><i class="fa fa-phone"> (774) 420-6185</i></a>
</div>
<div class="socialMedia">
    <a href=""><i class="fa fa-facebook"></i></a>
    <a href=""><i class="fa fa-instagram"></i></a>
    <a href=""><i class="fa fa-twitter"></i></a>
    <a href=""><i class="fa fa-linkedin"></i></a>
</div>
</nav>
<!-- main navbar -->
 <div>
<nav class="MainNav" style=" border: 1px solid black">
    <div class="row">
        <div class="col-sm-2"><router-link class="title" to="/"><h2 class="shopName">Carter</h2></router-link></div>
        <div class="col-sm-8 a">
            <ul>
                <router-link class="link" to="/">Home</router-link>
                <router-link class="link" to="/about">About</router-link>
                <router-link class="link" to="/shop">Shop</router-link>
                <router-link class="link" to="/contact">Contact</router-link>
            </ul>
        </div>
        <div class="col-sm-2 socials">
            <a href=""><i class="fa fa-search"></i></a>
            <a href=""><i class="fa fa-cart-arrow-down"><span class="num">7</span></i></a>
            <a href=""><i class="fa fa-user"></i><span class="user">99</span></a>
        </div>
    </div>
</nav> 
    <!-- media queries -->
   <div class="mobile-nav">
        <div class="col-sm-6">
            <div class="col-sm-2"><router-link class="title" to="/"><h2 class="shopName">Carter</h2></router-link></div>
        </div>
        <div class="col-sm-6">
            <div @click="toggleMobileNav()"><i  class="fa fa-bars"></i></div>
        </div>
   </div>
   <transition name="expand">
        <ul class="mobileView"  v-show="mobile"> 
            <ul class="dropdown-nav">
                <router-link class="link" to="/">Home</router-link>
                <router-link class="link" to="">About</router-link>
                <router-link class="link" to="">Shop</router-link>
                <router-link class="link" to="">Contact</router-link>
            </ul>
            <ul class="mobileViewSocials">
            <input type="text" placeholder="search..."><button><a href=""><i class="fa fa-search"></i></a></button>
            <a href=""><i class="fa fa-cart-arrow-down"><span class="num">7</span></i></a>
            <a href=""><i class="fa fa-user"><span class="user">99</span></i></a>
        </ul>
     </ul>
    </transition>
</div> 

</body>
</template>

<script>
    //  import { CollapseTransition } from "@ivanv/vue-collapse-transition"
export default {
    data() {
        return {
            mobile: false,
            expand: 'fade'
        }
    },
    methods: {
        toggleMobileNav() {
            this.mobile = !this.mobile
        },
    },
}
</script>

<style scoped>
.TopMostNav {
    display: flex;
    justify-content: space-between;
    background-color: #212934;
    padding: 1rem 15rem;
}
.TopMostNav a {
       color: #cfd6e1;
       margin: 1rem;
       font-size: 12px;
}

.MainNav {
    padding: 0;
    height: 15vh;
    overflow: hidden;
    box-shadow: 5px 3px 10px rgb(218, 214, 214) !important;
}

.col-sm-6, .socials a {
    margin: 3rem 0;
}
.row {
    display: flex;
    justify-content: space-between;
    height: 12vh;
    margin: auto 15rem auto 10rem;
}
.MainNav .a {
    margin: auto;
}

.shopName {
    color: #59ab6e;
    padding: 5px 0;
    font-size: 48px;
}

.link {
    margin: 0 5rem;
    font-size: 18px;
    color: #212934 !important;
}

.link:hover, .title:hover {
    color: #59ab6e !important;
    text-decoration: none;
}


.socials {
    display: flex;
    justify-content: space-evenly;
    margin: auto 3px auto 3px !important;
    font-size: 20px;
}
 .socials a {
    color: black;
 }


.socials .user {
     border-radius: 40%;
}

span {
    position: absolute;
    background-color: #e9eef5;
    border-radius: 50%;
    padding: 3px 8px;
    top: 1.5rem; 
    margin-left: 0;
}

.MediaQueries {
    display: none;
}

.fa-bars {
    font-size: 34px;
    margin: 4rem auto 0 15rem;
    color: #c5c7ca;
}

/* Mobile nav */
.mobile-nav {
     display: none;
     top: 12vh;
     padding: 0 1rem 9rem 1rem;
     box-shadow: 5px 3px 10px rgb(218, 214, 214);
     height: 10vh;
}
 .mobile-nav div {
    margin: 0 auto 4rem auto;
 }
.mobileView {
    display: none;
     padding: 0 1rem 3rem 1rem;
     height: auto;
     text-align: left;
}

.dropdown-menu {
    display: block;
}
.dropdown-nav a {
    display: block !important;
}

.mobileViewSocials .fa {
font-size: 18px;
color: black
}

.mobileViewSocials .fa-cart-arrow-down, .mobileViewSocials .fa-user {
    margin-left: 1rem;
    font-size: 22px;
}
.mobileViewSocials .fa-user {
    margin-left: 3rem;
}

.mobileViewSocials span {
    top: 35rem;
}
input {
    width: 50%;
    padding: 6px 12px;
    border-top-left-radius: 5px;
    border-bottom-left-radius: 5px;
}
input, button {
       border: 1px solid rgb(204, 204, 204);
       height: 40px;
}
button {
      background-color: #e9ecef;
       width: 50px;
       border-top-right-radius: 5px;
       border-bottom-right-radius: 5px;
}
.expand-enter-from{
    opacity: 0;
}
.expand-enter-to{
    opacity: 1;
}
.expand-enter-active{
    transition: all 2s ease;
}
/* end */

@media  (max-width: 1200px) {
    .row {
         margin: auto 8rem auto 5rem;
    }
    .link {
         margin: 3.5rem 2rem;
    }
}

@media  (max-width: 992px) {
    .MainNav {
        display: none;
    }

    .mobile-nav{
        display: block;
        overflow: hidden;
    }
    .TopMostNav {
        display: none;
    }
    .mobileView{
        display: block;
    }
}

@media only screen and (max-width: 600px) {
     .mobile-nav{
        display: flex;
        justify-content: space-around;
        overflow: hidden;
        padding-bottom: 10rem;
    }
    .mobile-nav div {
        margin: auto 0;
    }

    .fa-bars {
        margin-right: 2rem;
    }
}
</style>