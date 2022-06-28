<template>
<main>
   <div id="myCarousel" class="carousel slide" data-ride="carousel">
    <!-- Indicators -->
      <ol class="carousel-indicators">
        <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
        <li data-target="#myCarousel" data-slide-to="1"></li>
        <li data-target="#myCarousel" data-slide-to="2"></li>
      </ol>

      <!-- Wrapper for slides -->
      <div class="carousel-inner">
        <div class="item active">
          <div class="row"> 
          <div class="col-sm-6 text">
            <h2 class="title"><strong style="color: #59ab6e;">Carter's</strong> Sneaker Shop</h2>
              <h4>Hot and affordable Kicks</h4>
              <p>Carter's Sneaker Shop is a dedicated online store which deals in authentic and affordable shoes. Discover new collection Shoes and sneakers right here at your convenience.</p>
          </div>
          <div class="col-sm-6">
              <img src="../assets/shoe.jpg" alt="">
          </div>
          </div>
        </div>

        <div class="item">
            <div class="row">
            <div class="col-sm-6 text">
                <h2>Clothes and accessories</h2>
                <h4>Authentic and Quality Clothing, Watches, etc</h4>
                <p>We bring you a variety of high quality products to suit all your occasions.</p>
            </div>
            <div class="col-sm-6">
                  <img src="../assets/lamp.jpg" alt="">
            </div>
          </div>
        </div>
      
        <div class="item">
            <div class="row">
            <div class="col-sm-6 text">
                <h2 class="title">Carter's Sneaker Shop</h2>
                <h4>Hot and affordable Kicks</h4>
                <p>Carter's Sneaker Shop is a dedicated online store which deals in authentic and affordable shoes. Discover new collection Shoes and sneakers right here at your convenience.</p>
            </div>
            <div class="col-sm-6">
                <img src="../assets/shoe.jpg" alt="">
            </div>
          </div>
        </div>
      </div>

      <!-- Left and right controls -->
      <a class="left carousel-control" href="#myCarousel" data-slide="prev">
        <span class="glyphicon glyphicon-chevron-left"></span>
        <span class="sr-only">Previous</span>
      </a>
      <a class="right carousel-control" href="#myCarousel" data-slide="next">
        <span class="glyphicon glyphicon-chevron-right"></span>
        <span class="sr-only">Next</span>
      </a>
  </div>

<!-- categories section -->
  <div class="categories-section">
    <h2>Categories of The Month</h2>
    <p>Most purchased items of the month.</p>

    <div class="row2">
      <div class="col-sm-4">
        <img src="../assets/watches.jpg" alt="">
        <p><strong>Watches</strong></p>
        <button>Go Shop</button>
      </div>
      <div class="col-sm-4">
        <img src="../assets/shoes.jpg" alt="">
        <p><strong>Shoes</strong></p>
        <button>Go Shop</button>
      </div>
      <div class="col-sm-4">
        <img src="../assets/glasses.jpg" alt="">
        <p><strong>Accessories</strong></p>
        <button>Go Shop</button>
      </div>
    </div>
  </div>
  <!-- end of categories -->
  <!-- cards(featured products) -->
  <div class="featured-product">
      <h2>Featured Product</h2>
      <p>Special items on Sale.</p>

      <div class="row3">
            <div class="col-sm-4">
              <div class="card" style="width:400px">
                      <router-link to=""><img class="card-img-top" src="../assets/gym.jpg" alt="Card image"></router-link>
              <div class="card-body">
                <div class="rating">
                <div class="col-sm-6 stars">
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star" style="color: #e9eef5;"></i>
                <i class="fa fa-star" style="color: #e9eef5;"></i>
                </div>
                <div class="col-sm-6 num" ><p>$240.00</p></div>
                </div>
                
                <h3 class="card-title">Gym Weight</h3>
                <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sunt in culpa qui officia deserunt.</p>
               <h4>Reviews (74)</h4>
              </div>
            </div>
          </div>
            <div class="col-sm-4">
              <div class="card" style="width:400px">
                      <router-link to=""><img class="card-img-top" src="../assets/feature_prod_02.jpg" alt="Card image"></router-link>
              <div class="card-body">
                 <div class="rating">
                <div class="col-sm-6 stars">
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star" style="color: #e9eef5;"></i>
                <i class="fa fa-star" style="color: #e9eef5;"></i>
                </div>
                <div class="col-sm-6 num" >
                  <p>$480.00</p>
                </div>
                </div>
                <h3 class="card-title">Cloud Nike Shoes</h3>
                <p class="card-text">Aenean gravida dignissim finibus. Nullam ipsum diam, posuere vitae pharetra sed, commodo ullamcorper.</p>
                <h4>Reviews (48)</h4>
              </div>
            </div>
          </div>
          <div class="col-sm-4">
              <div class="card" style="width:400px">
              <router-link to=""><img class="card-img-top" src="../assets/glasses.jpg" alt="Card image"></router-link>
              <div class="card-body">
                 <div class="rating">
                <div class="col-sm-6 stars">
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                </div>
                <div class="col-sm-6 num" ><p>$360.00</p></div>
                </div>
                <h3 class="card-title">Summer Addides Shoes</h3>
                <p class="card-text">Curabitur ac mi sit amet diam luctus porta. Phasellus pulvinar sagittis diam, et scelerisque ipsum lobortis nec.</p>
                <h4>Reviews (24)</h4>
              </div>
            </div>
          </div>
      </div>
    </div>
  <!-- end -->
    
</main>
</template>

<style scoped>
/* Carousel */
main {
  overflow: hidden;
}
.carousel {
    background-color: #efefef;
    height: 60vh;
}

.carousel-inner {
  height: 100%;
}
.carousel-inner .row{
    display: flex;
    justify-content: space-between;
    padding-top: 5rem;
}

.carousel .row img {
  width: 80%;
}

.title {
  color: #67b27a;
  font-size: 40px;
}
.text {
  text-align: center;
}
/* end of carousel */
/* Categories section */
.categories-section {
  margin: 5rem auto;
}
.row2 {
  display: flex;
  justify-content: space-between;
}

.row2 img {
  width: 60%;
  border-radius: 50%;
  object-fit: cover;
  object-position: center;
  margin: 3rem 0;
}

.row2 .col-sm-4 p {
  font-size: 20px !important;
}
.row2 .col-sm-4 button {
  width: 100px;
  height: 40px;
  border-radius: 5px;
  background-color: #59ab6e;
  border: none;
  color: white;
  font-size: 16px;
}
/* end */

/* featured product */
.featured-product {
  background-color: #e9eef5;
  padding: 1rem;
}

.row3 {
  display: flex;
  justify-content: space-between !important;
  flex-wrap: wrap;
}
.row3 .col-sm-4 img{
  width: 100%;
  height: 300px;
   border-top-left-radius: 10px;
  border-top-right-radius: 10px;
}
.card {
  background-color: white;
  height: 550px;
  border-top-left-radius: 20px;
  border-top-right-radius: 20px;
}
.rating {
  display: flex;
  justify-content: space-evenly;
}
.stars {
  font-size: 20px;
  color: rgb(224, 224, 12);
}
.card h4, p {
  text-align: left;
  font-size: 18px;
  margin: 5px;
}
.card h4, .num {
  color: #c2c4c7;
}
</style>