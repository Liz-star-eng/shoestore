<template>
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
<div :class="{'scrolled-nav': scrollPosition}">
<nav class="MainNav">
    <div class="row">
        <div class="col-sm-2"><router-link class="title" to="/"><h2 class="shopName">Carter</h2></router-link></div>
        <div class="col-sm-8 a" v-show="!mobile">
            <ul>
                <router-link class="link" to="/">Home</router-link>
                <router-link class="link" to="">About</router-link>
                <router-link class="link" to="">Shop</router-link>
                <router-link class="link" to="">Contact</router-link>
            </ul>
        </div>
        <div class="col-sm-2 socials">
            <a href=""><i class="fa fa-search"></i></a>
            <a href=""><i class="fa fa-cart-arrow-down"><span class="num">7</span></i></a>
            <a href=""><i class="fa fa-user"><span class="user">99</span></i></a>
        </div>
    </div>
    <!-- media queries -->
    <div class="icon">
        <i @click="toggleMobileNav" v-show="mobile" class="fa fa-bars" :class="{'icon-active': mobileNav}"></i>
    </div>
    <transition name="mobile-nav">
        <ul class="mobileView">
                <div class="col-sm-2">
                  <router-link class="title" to="/"><h2 class="shopName">Carter</h2>
                  </router-link>
                </div>
            <ul v-show="mobile">
                <router-link class="link" to="/">Home</router-link>
                <router-link class="link" to="">About</router-link>
                <router-link class="link" to="">Shop</router-link>
                <router-link class="link" to="">Contact</router-link>
            </ul>
            <ul class="socials">
            <a href=""><i class="fa fa-search"></i></a>
            <a href=""><i class="fa fa-cart-arrow-down"><span class="num">7</span></i></a>
            <a href=""><i class="fa fa-user"><span class="user">99</span></i></a>
        </ul>
     </ul>
    </transition>
</nav>
</div>



</template>

<script>
export default {
    data() {
        return {
            scrollPosition: null,
            mobile: null,
            mobileView: null,
            windowWidth: null
        }
    },
    methods: {
        toggleMobileNav() {
            this.mobile = !this.mobile
        }
    }
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
    padding: 0 !important;
     box-shadow: 5px 3px 10px rgb(218, 214, 214);
     height: 12vh;
}

.row {
    display: flex;
    justify-content: space-between;
    height: 12vh;
    margin: auto 15rem auto 10rem;
    overflow: hidden;
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
    margin: auto;
    font-size: 18px;
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
    padding: 2px 8px;
    top: 0; 
}

.MediaQueries {
    display: none;
}

.fa-bars {
    font-size: 34px;
    margin: 4rem auto 0 15rem;
    color: #c5c7ca;
}
.mobileView {
    display: none;
}

/* media queries */
@media screen and (max-width: 1024px) {
    .mobileView {
    display: flex;
    justify-content: space-between;
    height: 7vh;
    z-index: 1;
    background-color: #212934;
}
.TopMostNav {
    display: none;
}
.MainNav {
    display: none;
}

}
</style>