<template>
  <div id="gallery ">
    <div class="text-center H900 N600 my-10">Gallery</div>
    <div class="row ">
      <div class="column ">
        <img src="https://res.cloudinary.com/dcyay2pow/image/upload/v1680935528/photos/WhatsApp_Image_2023-04-05_at_7.11.06_PM_uv12ge.jpg" @click="openModal(1)" class="hover-shadow rounded-xl ">
        <img src="https://res.cloudinary.com/dcyay2pow/image/upload/v1680935529/photos/WhatsApp_Image_2023-04-05_at_7.11.50_PM_p1zr1y.jpg" @click="openModal(2)" class="hover-shadow rounded-xl">
        <img src="https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/WhatsApp_Image_2023-04-05_at_7.37.48_PM_xx5ia1.jpg" @click="openModal(3)" class="hover-shadow rounded-xl">
      </div>
      <div class="column">
        <img src="https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/WhatsApp_Image_2023-04-05_at_7.37.48_PM_xx5ia1.jpg" @click="openModal(4)" class="hover-shadow rounded-xl">
        <img src="https://res.cloudinary.com/dcyay2pow/image/upload/v1680935534/photos/WhatsApp_Image_2023-04-05_at_8.27.45_PM_bn3pzy.jpg" @click="openModal(5)" class="hover-shadow rounded-xl">
        <!-- <img src="https://res.cloudinary.com/akwaah/image/upload/v1680378377/IMG_20220219_124010_ibtdcs.jpg" @click="openModal(6)" class="hover-shadow rounded-xl"> -->
        
      </div>
      <!-- <div class="column">
        <img src="https://res.cloudinary.com/akwaah/image/upload/v1680380069/IMG_20220430_131109_1_fh6hqp.jpg" @click="openModal(7)" class="hover-shadow rounded-xl">
        <img src="https://res.cloudinary.com/akwaah/image/upload/v1680552211/HJ5A7709_nqqagu.jpg" @click="openModal(8)" class="hover-shadow rounded-xl">
        <img src="https://res.cloudinary.com/akwaah/image/upload/v1680380208/IMG_20220219_133542_1_x5b2ds.jpg" @click="openModal(9)" class="hover-shadow rounded-xl">
        <img src="https://res.cloudinary.com/akwaah/image/upload/v1680380196/IMG_20220430_131627_nduefu.jpg" @click="openModal(10)" class="hover-shadow rounded-xl">
      </div>
      <div class="column">
        <img src="https://res.cloudinary.com/akwaah/image/upload/v1680552203/HJ5A7706_spawij.jpg" @click="openModal(11)" class="hover-shadow rounded-xl">
        <img src="https://res.cloudinary.com/akwaah/image/upload/v1680645908/HJ5A7750_eswedq.jpg" @click="openModal(12)" class="hover-shadow rounded-xl">
        <img src="https://res.cloudinary.com/akwaah/image/upload/v1680380165/IMG_20220219_121336_pp0xmv.jpg" @click="openModal(13)" class="hover-shadow rounded-xl">
      </div> -->
     
    </div>

    <!-- The Modal/Lightbox -->
    <div id="myModal" class="modal" :style="{display: showModal ? 'block' : 'none' }">
      <span class="close cursor" style="z-" @click="closeModal">&times;</span>
      <div class="modal-content container">
        <div v-for="(img, index) in images" :key="index" class="mySlides" :style="{ display: index === currentSlideIndex ? 'flex' : 'none' }">
          <div class="numbertext">{{ index + 1 }} / {{ images.length }}</div>
          <div class="imgSlid">
          <img :src="img.src" style="" >
        </div>
        </div>

        <!-- Next/previous controls -->
        <a class="prev" @click="plusSlides(-1)">&#10094;</a>
        <a class="next" @click="plusSlides(1)">&#10095;</a>

        <!-- Caption text -->
        <!-- <div class="caption-container">
          <p id="caption">{{ images[currentSlideIndex].alt }}</p>
        </div> -->

        <!-- Thumbnail image controls -->
        <!-- <div class="row">
        <div class="column" v-for="(img, index) in images" :key="index">
          <img class="demo" :src="img.src" @click="currentSlide(index)" :alt="img.alt">
        </div>
      </div> -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showModal: false,
      currentSlideIndex: 0,
      images: [
        { src: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935528/photos/WhatsApp_Image_2023-04-05_at_7.11.06_PM_uv12ge.jpg", wideSrc: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/WhatsApp_Image_2023-04-05_at_7.37.48_PM_xx5ia1.jpg", alt: "Nature" },
        { src: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935529/photos/WhatsApp_Image_2023-04-05_at_7.11.50_PM_p1zr1y.jpg", wideSrc: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/WhatsApp_Image_2023-04-05_at_7.37.48_PM_xx5ia1.jpg", alt: "Snow" },
        { src: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/WhatsApp_Image_2023-04-05_at_7.37.48_PM_xx5ia1.jpg", wideSrc: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/WhatsApp_Image_2023-04-05_at_7.37.48_PM_xx5ia1.jpg", alt: "Mountains" },
        
        { src: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/WhatsApp_Image_2023-04-05_at_7.37.48_PM_xx5ia1.jpg", wideSrc: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/WhatsApp_Image_2023-04-05_at_7.37.48_PM_xx5ia1.jpg", alt: "Lights" },
        { src: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935534/photos/WhatsApp_Image_2023-04-05_at_8.27.45_PM_bn3pzy.jpg", wideSrc: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935534/photos/WhatsApp_Image_2023-04-05_at_8.27.45_PM_bn3pzy.jpg", alt: "Snow" },
        // { src: "https://res.cloudinary.com/akwaah/image/upload/v1680378377/IMG_20220219_124010_ibtdcs.jpg", wideSrc: "https://res.cloudinary.com/akwaah/image/upload/v1680203747/CG7A3084_ihsozw.jpg", alt: "Mountains" },
        
        // { src: "https://res.cloudinary.com/akwaah/image/upload/v1680380069/IMG_20220430_131109_1_fh6hqp.jpg", wideSrc: "https://res.cloudinary.com/akwaah/image/upload/v1680203721/CG7A3085_v2kbeh.jpg", alt: "Lights" },
        // { src: "https://res.cloudinary.com/akwaah/image/upload/v1680552211/HJ5A7709_nqqagu.jpg", wideSrc: "https://res.cloudinary.com/akwaah/image/upload/v1680203748/CG7A3054_njkkvb.jpg", alt: "Snow" },
        // { src: "https://res.cloudinary.com/akwaah/image/upload/v1680380208/IMG_20220219_133542_1_x5b2ds.jpg", wideSrc: "https://res.cloudinary.com/akwaah/image/upload/v1680203747/CG7A3084_ihsozw.jpg", alt: "Mountains" },
        // { src: "https://res.cloudinary.com/akwaah/image/upload/v1680380196/IMG_20220430_131627_nduefu.jpg", wideSrc: "https://res.cloudinary.com/akwaah/image/upload/v1680203721/CG7A3085_v2kbeh.jpg", alt: "Lights" },

        // { src: "https://res.cloudinary.com/akwaah/image/upload/v1680552203/HJ5A7706_spawij.jpg", wideSrc: "https://res.cloudinary.com/akwaah/image/upload/v1680203748/CG7A3054_njkkvb.jpg", alt: "Snow" },
        // { src: "https://res.cloudinary.com/akwaah/image/upload/v1680645908/HJ5A7750_eswedq.jpg", wideSrc: "https://res.cloudinary.com/akwaah/image/upload/v1680203747/CG7A3084_ihsozw.jpg", alt: "Mountains" },
        // { src: "https://res.cloudinary.com/akwaah/image/upload/v1680380165/IMG_20220219_121336_pp0xmv.jpg", wideSrc: "https://res.cloudinary.com/akwaah/image/upload/v1680203721/CG7A3085_v2kbeh.jpg", alt: "Lights" }

      ]
    };
  },
  methods: {
    // Open the Modal
    openModal(slideIndex) {
      this.showModal = true;
      this.currentSlideIndex = slideIndex - 1;
    },

    // Close the Modal
    closeModal() {
      this.showModal = false;
    },

    // Next/previous controls
    plusSlides(n) {
      this.currentSlideIndex += n;
      if (this.currentSlideIndex >= this.images.length) {
        this.currentSlideIndex = 0;
      } else if (this.currentSlideIndex < 0) {
        this.currentSlideIndex = this.images.length - 1;
      }
    },

    // Thumbnail image controls
    currentSlide(index) {
      this.currentSlideIndex = index;
    }
  },
  mounted() {
    // Show the first slide
this.currentSlideIndex = 0;
},
computed: {
currentSlide() {
return this.images[this.currentSlideIndex];
}
}
};
</script>
<style scoped>

.imgSlid {
    /* height: 50vh; */
    background-size: cover;
    aspect-ratio: 3/2;
    justify-content: center;
    display: flex;

    /* filter: blur(3px);
    -webkit-filter: blur(px); */
    /* background-attachment: fixed; */
  }


.row {
  display: flex;
  flex-wrap: wrap;
  padding: 0 4px;
}

/* Create four equal columns that sits next to each other */
.column {
  flex: 25%;
  max-width: 25%;
  padding: 0 4px;
}

.column img {
  margin-top: 8px;
  vertical-align: middle;
  width: 100%;
}

/* Responsive layout - makes a two column-layout instead of four columns */
@media screen and (max-width: 800px) {
  .column {
    flex: 50%;
    max-width: 50%;
  }
}

/* Responsive layout - makes the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 600px) {
  .column {
    flex: 100%;
    max-width: 100%;
  }
}

/* The Modal (background) */
.modal {
  display: none;
  position: fixed;
  z-index: 1;
  padding-top: 5rem;
  left: 0;
  top: 7%;
  width: 100vw;
  height: 100vh;
  /* overflow: auto; */
  background-color: rgb(0, 0, 0, 0.7);
}

/* Modal Content */
.modal-content {
  position: relative;
  background-color: #fefefe00;
  margin: auto;
  padding: 0;
  border: 0;
  /* width: 90%; */
  /* max-width: 1200px; */
}

/* The Close Button */
.close {
  color: white;
  position: absolute;
  top: 10px;
  right: 25px;
  font-size: 35px;
  font-weight: bold;
  cursor: pointer;
}

.close:hover,
.close:focus {
  color: #999;
  text-decoration: none;
  cursor: pointer;
}

/* Hide the slides by default */
.mySlides {
  /* display: flex; */
}

/* Next & previous buttons */
.prev,
.next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -50px;
  color: white;
  font-weight: bold;
  font-size: 20px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
  -webkit-user-select: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover,
.next:hover {
  background-color: rgba(0, 0, 0, 0.2);
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* Caption text */
.caption-container {
  text-align: center;
  background-color: black;
  padding: 2px 16px;
  color: white;
}

img.demo {
  opacity: 0.6;
  /* height: 50vh; */
}

.active,
.demo:hover {
  opacity: 1;
}

img.hover-shadow {
  transition: 0.3s;
}

.hover-shadow:hover {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}
</style>
