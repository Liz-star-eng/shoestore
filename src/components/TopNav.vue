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
<nav class="MainNav">
    <div class="row">
        <div class="col-sm-2"><router-link class="title" to=""><h2 class="shopName">Carter</h2></router-link></div>
        <div class="col-sm-8 a">
            <router-link class="link" to="">Home</router-link>
            <router-link class="link" to="">About</router-link>
            <router-link class="link" to="">Shop</router-link>
            <router-link class="link" to="">Contact</router-link>

        </div>
        <div class="col-sm-2 socials">
            <a href=""><i class="fa fa-search"></i></a>
            <a href=""><i class="fa fa-cart-arrow-down"></i><span class="cart">7</span></a>
            <a href=""><i class="fa fa-user"></i><span class="user">99</span></a>

        </div>
    </div>

</nav>
</template>

<style scope>
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
    margin: auto;
    font-size: 18px;
}
 .socials a {
    color: black;
 }
 span {
    position: absolute;
    background-color: #e9eef5;
    border-radius: 50%;
    padding: 2px 8px;
    top: 0;
}


.socials .user {
     border-radius: 40%;
}
</style>