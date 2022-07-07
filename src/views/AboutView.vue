<template>
 <main class="about-hero row">
  <div class="col-sm-6">
    <h2>About Us</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt est nemo quasi dicta rem vitae animi tempore possimus culpa magni nesciunt nulla, atque totam provident ea voluptate, blanditiis asperiores iure nam commodi rerum. Harum, fuga a! Atque iste, ullam voluptas illum sed earum porro molestias voluptatibus incidunt veritatis cum libero?</p>
  </div>
  <div class="col-sm-6">
    <img src="../assets/about-hero.svg" alt="">
  </div>
 </main>

 <div class="ourServices">
  <h1>Our Services</h1>
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, <br> sed do eiusmod Lorem ipsum dolor sit amet.</p>
  <div class="row2">
    <div class="col-sm-3">
      <i class="fa fa-truck"></i>
    </div>
    <div class="col-sm-3 arrow">
      <i class="fa fa-long-arrow-right"></i>
      <i class="fa fa-long-arrow-left" ></i>

    </div>
    <div class="col-sm-3">
      <i class="fa fa-percent"></i>
    </div>
    <div class="col-sm-3">
      <i class="fa fa-user"></i>
    </div>
  </div>
 </div>
 <div class="Brands">
    <h1>OUR BRANDS</h1>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, <br> sed do eiusmod Lorem ipsum dolor sit amet.</p>
    <div class="container">
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
                <div class="col-sm-3">
                  <img src="../assets/brand_01.png" alt="">
                </div>
                <div class="col-sm-3">
                  <img src="../assets/brand_02.png" alt="">
                </div>
                <div class="col-sm-3">
                  <img src="../assets/brand_03.png" alt="">
                </div>
                <div class="col-sm-3">
                  <img src="../assets/brand_04.png" alt="">
                </div>
              </div>
            </div>

            <div class="item">
                <div class="row"> 
                <div class="col-sm-3">
                  <img src="../assets/brand_01.png" alt="">
                </div>
                <div class="col-sm-3">
                  <img src="../assets/brand_02.png" alt="">
                </div>
                <div class="col-sm-3">
                  <img src="../assets/brand_03.png" alt="">
                </div>
                <div class="col-sm-3">
                  <img src="../assets/brand_04.png" alt="">
                </div>
              </div>
            </div>
          
            <div class="item">
              <div class="row"> 
                <div class="col-sm-3">
                  <img src="../assets/brand_01.png" alt="">
                </div>
                <div class="col-sm-3">
                  <img src="../assets/brand_02.png" alt="">
                </div>
                <div class="col-sm-3">
                  <img src="../assets/brand_03.png" alt="">
                </div>
                <div class="col-sm-3">
                  <img src="../assets/brand_04.png" alt="">
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
    </div>
 </div>
</template>

<style scoped>
main {
  background-color: #59ab6e;
  height: 500px;
  padding-top: 10rem;
}

.row {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}


h2, p {
  color: white;
  text-align: left;
}

p {
  font-size: 18px;
}

.row img {
  height: 300px;
}

/* Our services */
.ourServices {
  background-color: white;
  height: 500px;
}

.ourServices p, h1 {
  text-align: center;
  color: black;
}

.row2 {
  display: flex;
  justify-content: center;
  flex-direction: row;
  flex-wrap: wrap;
  width: 100%;
  padding-left: 20rem;
  padding-right: 20rem;
}
.row2 .col-sm-3 {
  box-shadow: 4px 3px 6px rgb(199, 197, 197);
  padding: 5rem 3rem !important;
  border-radius: 5px;
}

.row2 .col-sm-3 .fa {
  font-size: 60px;
  color: #59ab6e;
}

.row2 .col-sm-3:hover{
background-color: #59ab6e;
}

.arrow {
  display: flex;
  flex-direction: column;
}

/* Brands */
.Brands {
  height: 500px;
  background-color: #e9eef5;
  padding: 5px;
}

.Brands p, h1 {
  text-align: center;
  color: black;
}

.container {
  padding: 5rem;
}

.carousel-inner {
  padding: 10rem;
}
.carousel-control {
  background-color: #e9eef5 !important;
}
.row .col-sm-3 img {
  width: 50px;
  height: 50px;
}

</style>