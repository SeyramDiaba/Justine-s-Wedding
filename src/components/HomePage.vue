<template>
  <div >
    <div class="bgColor" data-bs-theme="light">
      <!-- banner Image -->
      <div class="overlay boderAroundT" style="">
        <div id="imgBanner" class="imgBanne center mx-auto " style="">
          <div class="gridinfo"></div>

          <div id="carouselExampleSlidesOnly" class="carousel slide" data-bs-ride="carousel">
  <div class="bgCool">
    <div class="carousel-item active ">
      <img src="https://res.cloudinary.com/dcyay2pow/image/upload/v1680954554/Brown_Modern_2_gjkpe0.png" class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="https://res.cloudinary.com/dcyay2pow/image/upload/v1680954384/Brown_Modern_Thank_You_Banner_Landscape_1_l1fdto.png" class="d-block w-100" alt="...">
    </div>
    <!-- <div class="carousel-item">
      <img src="https://res.cloudinary.com/akwaah/image/upload/v1680203747/CG7A3084_ihsozw.jpg" class="d-block w-100" alt="...">
    </div> -->
    <!-- <div class="carousel-item">
      <img src="https://res.cloudinary.com/akwaah/image/upload/v1680203755/CG7A3061_bvof1m.jpg" class="d-block w-100" alt="...">
    </div> -->
    <!-- <div class="carousel-item">
      <img src="https://res.cloudinary.com/akwaah/image/upload/v1680552203/HJ5A7706_spawij.jpg" class="d-block w-100" alt="...">
    </div> -->
  </div>
</div>
          
        </div>
        <!-- <div class="H900 imgCenter text-white" style="color: white !important;">
          #JojoGotBerta 2023
        </div> -->
        
          <div class="gridinfo"></div>
          <img
            src="https://res.cloudinary.com/dcyay2pow/image/upload/v1680951719/Floral_Wreath_Wedding_Monogram_Circle_Sticker_e2nqww.png"
            alt=""
            class="imgCenter"
            style="width:50vw"
          />
      </div>

      <!--Navbar  -->
      <!-- <nav class="navbar sticky-top bg-light N400 P200"> -->
      <Navbar />
      <!-- </nav> -->

      <!-- Who are we -->
      <WhoAreWe />

      <!-- count down timer -->
      <div class="countdow cente bgColor boderAroundB" style="">
        <!-- <Countdown end="April 22, 2023"></Countdown> -->
        <count-down-timer/>
      </div>

      <!-- about us -->
      <div class="boderAroundT">
      <AboutUs/>
    </div>
      

      <!-- when and where -->
      <div class="boderAroundB">
      <WhenAndWhere/>
    </div>
      


      <!-- RSVP -->
      <div id="rsvp" class="rsvp py-10 center boderAroundB">
        <div class="gridinfo"></div>
        <!-- <img src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/rsvp.jpg" width="1600" height="900" data-stellar-ratio="0.5" alt="" style="opacity: 1; transform: translate3d(0px, -128.409px, 0px); width: 1903px; height: 1070.44px; margin-top: -58.3827px; margin-left: 0px;"> -->
        <div class="container">
          <form action=""></form>
        </div>
      </div>

      <!-- Grooms and braidmaids -->
      <!-- <MenAndMaids/>
      <MenAndMaids/> -->

      <!-- Quotes -->
      <div class="boderAroundT">
      <Quotes/>
    </div>

    <photo-booth/>

      <!-- Photo Gallery -->
      <!-- <div class="boderAroundB">
      <PhotoGallerySection/>
    </div> -->

      <!-- Footer -->
      <!-- <FooterSection/> -->
      <!-- <audio controls>
  <source src="horse.ogg" type="audio/ogg">
Your browser does not support the audio element.
</audio> -->
    </div>
  </div>
</template>

<script>
import Navbar from './HomePageComp/Navbar.vue'
import AboutUs from './HomePageSection/AboutUs.vue'
import MenAndMaids from './HomePageSection/MenAndMaids.vue'
import Quotes from './HomePageSection/Quotes.vue'
import WhenAndWhere from './HomePageSection/WhenAndWhere.vue'
import WhoAreWe from './HomePageSection/WhoAreWe.vue'
import FooterSection from './HomePageSection/FooterSection.vue'
import PhotoGallerySection from './HomePageSection/PhotoGallerySection.vue'
import PhotoBooth from './HomePageSection/PhotoBooth.vue'
import CountDownTimer from './HomePageSection/CountDownTimer.vue'

export default {
  name: 'WeddingHomePage',
  data() {
    return {}
  },
  mounted() {},
  methods: {},
  components: {  Navbar, WhoAreWe, AboutUs, WhenAndWhere, MenAndMaids, Quotes, PhotoGallerySection, FooterSection, PhotoBooth, CountDownTimer }
}
</script>

<style >
@import url('https://fonts.googleapis.com/css2?family=Alex+Brush&display=swap');

.bgColor {
  background-color: #ecfbff;
}

.bgNav {
  background-color: #d0edf5;
}

.bgColor2 {
  background-color: #b13a1a15;
}

.imgCenter {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);

}

.boderAroundT {
  /* border-radius: 0 1rem 1rem 0rem; 
  border: 0.3rem solid #b13a1a; 
  border-left: 0px; 
  border-bottom: 0.3rem */
}

.boderAroundB {
  /* border-radius: 1rem 0rem 0rem 1rem; 
  border: 0.3rem solid #b13a1a;
  border-right: 0;
  border-bottom: 0.3rem */
}

.gridinfo {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  background: rgba(0,0,0,0.3);
  text-align: center;
  transition: all 0.8s;
}

/* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {
}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
}

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {
    
}

/* Extra large devices (large laptops and desktops, 1200px and up) */
/* @media only screen and (min-width: 1200px) { */
  .center {
    justify-content: center;
    align-items: center;
    display: flex;
  }
  .imgBanner {
    /* height: 100vh; */
    /* width: 100vw; */
    /* background-color: #d0edf530; */
    /* background-image: url(https://res.cloudinary.com/akwaah/image/upload/v1680203747/CG7A3084_ihsozw.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    filter: blur(1px); */
  /* -webkit-filter: blur(3px); */
  

  }

  
  .overlay {
  
  }

  .bgCool {
  object-fit: cover;
  width: 100%;
  height: 100%;
}
  .stickyNavbar {
    /* height: 7rem; */
    /* background-color: grey; */
  }
  .whoWeAre {
    /* height: 60vh; */
    /* background-color: red; */
  }
  .countdown {
    height: 10rem;
  }
  .aboutUs {
    /* height: 120vh; */
  }

  .brideGroomImage {
    /* height: 43.5vh; */
    background-repeat: no-repeat;
    background-size: contain;
    background-position: center center;
  }
  .whenNwhere {
    /* height: 90vh; */
  }
  .map {
    /* height: 60vh; */
  }
  .giftRegistry {
    height: 40vh;
  }

  .rsvp {
    height: 120vh;
    background-image: url(https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/rsvp.jpg);
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: cover;
  }

  .avatar {
    /* width: 20rem;
    height: 20rem; */
  }

  .menAndMaids {
    /* height: 50vh; */
  }

  .quotes {
    height: 50vh;
    background-image: url(https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/quote.jpg);
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: cover;
    font-style: italic;
  }

  .footer {
    /* height: 75vh; */
    background-image: url(https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/rsvp.jpg);
    background-repeat: no-repeat;
  }

  .footerImage {
    height: 5rem;
  }
/* } */
</style>
