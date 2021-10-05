<template>
  <div class="Site " >
    <!-- Button trigger modal -->
    
 <nav class="navbar navbar-expand-lg navbar-light bg-light rounded fixed-top">

    <a class="navbar-brand" href="#"><img src="img/logo.png" style="width: 60px; height: 50px" />أحجزلي</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarsExample09" aria-controls="navbarsExample09" aria-expanded="false" aria-label="Toggle navigation">
      <span style="font-size: 30px; cursor: pointer" 
          ><svg
            xmlns="http://www.w3.org/2000/svg"
            width="22"
            height="22"
            fill="currentColor"
            class="bi bi-list-nested"
            viewBox="0 0 16 16"
          >
            <path
              fill-rule="evenodd"
              d="M4.5 11.5A.5.5 0 0 1 5 11h10a.5.5 0 0 1 0 1H5a.5.5 0 0 1-.5-.5zm-2-4A.5.5 0 0 1 3 7h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm-2-4A.5.5 0 0 1 1 3h10a.5.5 0 0 1 0 1H1a.5.5 0 0 1-.5-.5z"
            /></svg></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarsExample09">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item active">
          <a class="nav-link" href="#">الصفحة الرئيسية</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">من نحن </a>
        </li>
        <li class="nav-item">
          <a class="nav-link " href="#" >تواصل معنا </a>
        </li>
      </ul>
  
    </div>
  </nav>

  <!-- end nav bar-->


<div class="contanier">
  <div class="row">
     <div class="col-12 col-md-5 mrtop">
       <h2> الموقع الاول في سوريا للرحلات </h2>
       <p> في هذا الموقع سوف نأخذك في جولة للعديد من الاماكن 
         <br>التي قد ترغب في زيارتها 
         كما سوف نساعدك في أختيار افضل الاماكن منها 
       </p>
       <span style="color:#4CAF50">نتمنى لك جولة سعيدة !!</span>
       </div>
    <div class="col-12 col-md-5 mrtopc">
  <img src="img/car.png" class="car">
</div>
  </div></div>


<br>
<br>
<br>
<section class="papular">
   <h2>المواقع الاكثر حجزا :</h2>
  </section>
  <div  class="container-fluid overflow-auto bg-custom">
  
 <div class="row d-flex flex-row flex-nowrap">
  <div
            class="col-12 col-md-3 col-sm-4"
            v-for="(cteg, i) in items"
            :key="i"
          >
            <div class="card mb-4 shadow-sm item" >
              <img :src="cteg.photo_center" height="225" class="img-card" />
              <div class="card-body">
                <h5 class="text-success">
                  {{ cteg.name }}
                </h5><br>
                <p class="card-text">
                  السعر:{{ cteg.price_discount }}
                </p>
                <div class="d-flex justify-content-between align-items-center">
                  <div class="d-flex">
                    <span style="font-size: 12px; color: #9e9e9e"
                      >تم النشر :{{ cteg.created_at }}</span
                    >
                    <button type="button" class="btn btn-sm btn-success mx-1">
                      التفاصيل
                    </button>
                    <button type="button" class="btn btn-sm btn-primary mx-1">
                      الحجز
                    </button>
                  </div>
                </div>
              </div>
            </div>
          </div></div></div>
<br>
<br>
<br>
<section class="papular">
          <h2>العروض والحسوم:</h2></section><br>
            <div class="container-fluid overflow-auto bg-custom">
        <div class="row d-flex flex-row flex-nowrap ">
          <div
            class="col-12 col-md-3 col-sm-4"
            v-for="(cteg, i) in disc"
            :key="i"
          >
            <div class="card mb-4 shadow-sm">
              <img :src="cteg.photo_center" height="225" class="img-card" />
              <div class="card-body">
                <h5 class="text-success">
                  {{ cteg.name }}
                </h5>
                <p class="card-text">
                  قبل الحسم: <del>{{ cteg.price }}</del
                  ><br />
                  السعر بعد الحسم:{{ cteg.price_discount }}
                </p>
                <div class="d-flex justify-content-between align-items-center">
                  <div class="d-flex">
                    <span style="font-size: 12px; color: #9e9e9e; display: block;"
                      >تم النشر :{{ cteg.created_at }}</span
                    >
                    <button type="button" class="btn btn-sm btn-success mx-1">
                      التفاصيل
                    </button>
                    <button type="button" class="btn btn-sm btn-primary mx-1">
                      الحجز
                    </button>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>



      <!-- Ui cards -->
        <section id="cards">
            <div class="container py-2">
                <div class="row pb-4">
                    <div class="col-12 text-center">
                        <div class="display-3">Our Team</div>
                    </div>
                </div>
                <!-- cards -->
                <div class="row">
                    <div class="col-lg-4 col-md-6 mb-4 pt-5">
                        <div class="card shadow-sm border-0">
                            <div class="card-body">
                                <div class="user-picture">
                                    <img src="https://images.unsplash.com/photo-1495603889488-42d1d66e5523?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=130&ixid=eyJhcHBfaWQiOjF9&ixlib=rb-1.2.1&q=80&w=130" class="shadow-sm rounded-circle" height="130" width="130" />
                                </div>
                                <div class="user-content">
                                    <h5 class="text-capitalize user-name">Carry Johnshon</h5>
                                    <p class=" text-capitalize text-muted small blockquote-footer">Web developer</p>
                                    <div class="small">
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star-half-alt text-warning"></i>
                                        <i class="fas fa-star text-light"></i>
                                    </div>
                                    <p class="small text-muted mb-0">Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet nemo harum repellendus aut itaque. Temporibus quaerat dolores ut, cupiditate molestiae commodi! Distinctio praesentium, debitis aut minima doloribus earum
                                        quia commodi.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-4 col-md-6 mb-4 pt-5">
                        <div class="card shadow-sm border-0">
                            <div class="card-body">
                                <div class="user-picture">
                                    <img src="https://images.unsplash.com/photo-1582003457856-20898dd7e1ea?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=130&ixid=eyJhcHBfaWQiOjF9&ixlib=rb-1.2.1&q=80&w=130" class="shadow-sm rounded-circle" height="130" width="130" />
                                </div>
                                <div class="user-content">
                                    <h5 class="text-capitalize user-name">Alex Carry</h5>
                                    <p class=" text-capitalize text-muted small blockquote-footer">Web developer</p>
                                    <div class="small">
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star-half-alt text-warning"></i>
                                        <i class="fas fa-star text-light"></i>
                                        <i class="fas fa-star text-light"></i>
                                    </div>
                                    <p class="small text-muted mb-0">Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet nemo harum repellendus aut itaque. Temporibus quaerat dolores ut, cupiditate molestiae commodi! Distinctio praesentium, debitis aut minima doloribus earum
                                        quia commodi.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-4 col-md-6 mb-4 pt-5">
                        <div class="card shadow-sm border-0">
                            <div class="card-body">
                                <div class="user-picture">
                                    <img src="https://images.unsplash.com/photo-1492447166138-50c3889fccb1?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=130&ixid=eyJhcHBfaWQiOjF9&ixlib=rb-1.2.1&q=80&w=130" class="shadow-sm rounded-circle" height="130" width="130" />
                                </div>
                                <div class="user-content">
                                    <h5 class="text-capitalize user-name">John Smith</h5>
                                    <p class=" text-capitalize text-muted small blockquote-footer">Web developer</p>
                                    <div class="small">
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star-half-alt text-warning"></i>
                                    </div>
                                    <p class="small text-muted mb-0">Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet nemo harum repellendus aut itaque. Temporibus quaerat dolores ut, cupiditate molestiae commodi! Distinctio praesentium, debitis aut minima doloribus earum
                                        quia commodi.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-4 col-md-6 mb-4 pt-5">
                        <div class="card shadow-sm border-0">
                            <div class="card-body">
                                <div class="user-picture">
                                    <img src="https://i.picsum.photos/id/836/130/130.jpg?hmac=Sot_REUw5W-XSuE6FmCjT9JenhZfiNqZYs3AQbfrZsc" class="shadow-sm rounded-circle" height="130" width="130" />
                                </div>
                                <div class="user-content">
                                    <h5 class="text-capitalize user-name">George Alex</h5>
                                    <p class=" text-capitalize text-muted small blockquote-footer">Web developer</p>
                                    <div class="small">
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star-half-alt text-warning"></i>
                                        <i class="fas fa-star text-light"></i>
                                        <i class="fas fa-star text-light"></i>
                                        <i class="fas fa-star text-light"></i>
                                    </div>
                                    <p class="small text-muted mb-0">Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet nemo harum repellendus aut itaque. Temporibus quaerat dolores ut, cupiditate molestiae commodi! Distinctio praesentium, debitis aut minima doloribus earum
                                        quia commodi.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-4 col-md-6 mb-4 pt-5">
                        <div class="card shadow-sm border-0">
                            <div class="card-body">
                                <div class="user-picture">
                                    <img src="https://images.unsplash.com/photo-1495603889488-42d1d66e5523?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=130&ixid=eyJhcHBfaWQiOjF9&ixlib=rb-1.2.1&q=80&w=130" class="shadow-sm rounded-circle" height="130" width="130" />
                                </div>
                                <div class="user-content">
                                    <h5 class="text-capitalize user-name">Carry Johnshon</h5>
                                    <p class=" text-capitalize text-muted small blockquote-footer">Web developer</p>
                                    <div class="small">
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star-half-alt text-warning"></i>
                                        <i class="fas fa-star text-light"></i>
                                    </div>
                                    <p class="small text-muted mb-0">Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet nemo harum repellendus aut itaque. Temporibus quaerat dolores ut, cupiditate molestiae commodi! Distinctio praesentium, debitis aut minima doloribus earum
                                        quia commodi.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-4 col-md-6 mb-4 pt-5">
                        <div class="card shadow-sm border-0">
                            <div class="card-body">
                                <div class="user-picture">
                                    <img src="https://images.unsplash.com/photo-1582003457856-20898dd7e1ea?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=130&ixid=eyJhcHBfaWQiOjF9&ixlib=rb-1.2.1&q=80&w=130" class="shadow-sm rounded-circle" height="130" width="130" />
                                </div>
                                <div class="user-content">
                                    <h5 class="text-capitalize user-name">Alex Carry</h5>
                                    <p class=" text-capitalize text-muted small blockquote-footer">Web developer</p>
                                    <div class="small">
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star text-warning"></i>
                                        <i class="fas fa-star-half-alt text-warning"></i>
                                        <i class="fas fa-star text-light"></i>
                                        <i class="fas fa-star text-light"></i>
                                    </div>
                                    <p class="small text-muted mb-0">Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet nemo harum repellendus aut itaque. Temporibus quaerat dolores ut, cupiditate molestiae commodi! Distinctio praesentium, debitis aut minima doloribus earum
                                        quia commodi.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <!-- /cards -->
        </section>
        <!-- /Ui cards -->






  </div>
</template>

<script>
// @ is an alias to /src
import axios from 'axios';

export default {
  name: "Site",
  components: {},
  created(){
    this.getItem();
    this.getdisc();
  },
  data() {
    return {
      items: [],
      disc:[]
    }},
     methods:{
      getItem() {
      axios
        .get("http://localhost:8000/api/Show-item-home")
        .then((response) => {
          console.log(response.data);
          this.items = response.data;
        })
        .catch((error) => {
          console.log(error);
        });
    
  },
   getdisc() {
      axios
        .get("http://localhost:8000/api/Show-item-discount")
        .then((response) => {
          console.log(response.data);
          this.disc = response.data;
        })
        .catch((error) => {
          console.log(error);
        });
    
  }
}};

</script>
<style scoped >
.Site{
  padding-left: 16px;
  padding-right: 16px;
  height: 5000px;

}
.car{
  animation: mymove 5s infinite;
  width: 600px;
  height: 600px;
}
@keyframes mymove {
  0%,100%{padding-bottom: 25px;padding-top: 0px;}
  50% {padding-top: 25px;padding-bottom: 0px;}
}
@media(max-width:650px){
  .car{
    width: 450px;
    height: 450px;
  }
}
@media(max-width:400px){
  .car{
    width: 370px;
    height: 370px;
  }
}
.mrtopc{
 margin-top: 50px
}
.mrtop{
    margin-top: 200px;
  }
@media(min-width:769px){
  .mrtop{
    margin-top: 250px;
  }
}

.papular{
      text-align: right;
}
.bg-custom{
    background-color: #def5c2;
       padding: 50px 50px 25px 50px;
    border-radius: 15px;
}
 /********************* Our Team ***************************** */

 /* ==== Cards using Bootstrap === */

#cards .card {
    border-radius: 20px;
    min-height: 100%;
}

#cards .heading-border {
    position: absolute;
    width: 100%;
    top: 60%;
}

#cards .card .user-picture img {
    position: absolute;
    top: -20%;
    right: 10%;
    background: #f8f9fa!important;
    padding: 10px;
}

#cards .card .user-content .user-name {
    margin-right: 150px;
}
</style>
