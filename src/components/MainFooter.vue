<template>
<footer>
    <div class="row">
        <div class="col-sm-4">
            <h2 class="CarterShop">Cater Shop</h2> <br>
            
            <a href=""><i class="fa fa-phone"></i> (774) 420-6185</a> <br><br>
            <a href=""><i class="fa fa-envelope"></i> jcsnkrs800@gmail.com</a>
        </div>
        <div class="col-sm-4">
            <h2>Products</h2><br>
        
            <router-link to="">Shoe</router-link><br><br>
            <router-link to="">Clothing</router-link><br><br>
            <router-link to="">Accessories</router-link><br>

        </div>
        <div class="col-sm-4">
            <h2>Further Info</h2><br>
           
            <router-link to="">Home</router-link><br><br>
            <router-link to="">About Us</router-link><br><br>
            <router-link to="">FAQS</router-link><br><br>
            <router-link to="">Contact</router-link><br>
        </div>
    </div>
    <div class="interact">
        <div class="socialMedia">
            <a href=""><i class="fa fa-facebook"></i></a>
            <a href=""><i class="fa fa-instagram"></i></a>
            <a href=""><i class="fa fa-twitter"></i></a>
            <a href=""><i class="fa fa-linkedin"></i></a>
        </div>
        <div class="email">
            <input type="email" placeholder="Email address">
            <button>Suscribe</button>
        </div>
    </div> 
    <div class="copyright">
<p>Copyright © Jay Carter's Sneaker Hub | Designed by Sean_or_Tony</p>
    </div>
</footer>

</template>

<style scoped>
footer {
    background-color: #212934;
    color: #cfd6e1;
    padding: 10px 0 0;
}
 h2 {
    border-bottom: 1px solid rgba(207, 214, 225, 0.3);
    padding: 5px;
 }
.CarterShop {
 color: #59ab6e;
}
 a {
    color: #cfd6e1;
    margin-bottom: 5px !important;
}

a:hover {
    color: #59ab6e;
    text-decoration: none;
}
.row {
display: flex;
justify-content: space-evenly;
padding: 5px;
height: 20%;
border-bottom: 1px solid rgba(207, 214, 225, 0.3);
}
.interact {
    display: flex;
    justify-content: space-between;
    margin: 5rem 20rem;
}
.interact a {
    margin: auto 5px;
    font-size: 18px;
    border: 1px solid rgba(207, 214, 225, 0.3);
    border-radius: 50%;
    padding: 1rem;
}
.interact a:first-child {
    padding: 1rem 1.3rem;
}

.email input, button {
    height: 40px;
    padding: 6px 12px;

}

.email input {
    background-color: #212934;
    border: solid 1px rgba(207, 214, 225, 0.3);
    border-top-left-radius: 5px;
    border-bottom-left-radius: 5px;
}

.email button {
    background-color: #59ab6e;
    width: 100px;
    border: none;
    border-top-right-radius: 5px;
    border-bottom-right-radius: 5px;
}

.copyright {
    text-align: left;
    background-color: #1d242d;
    padding: 3rem;
    font-size: 18px; 
}

</style>