<template>
    <div id="aboutUs" class="aboutUs  p-10 container bg-transparent" >
          <div class="borde text-center H900 N600 pb-10">Groom & Bride</div>

          <div class="row  ">
            <div
              class="col-md-6 col-lg-4  p-0 brideGroomImage rounded-xl">
            <div class="gridinfo rounded-xl"></div>
              <!-- <img src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/about-groom-540x405.jpg" alt="" srcset=""> -->
            </div>
            <div class="col-md-6 col-lg-8 my-auto p-10  ">
              <ProfileCard :aboutUs="groom"/>
            </div>
            <div class="col-md-6 col-lg-8  my-auto p-10 py-10 d-none d-md-block ">
                <ProfileCard :aboutUs="bride"/>
              
            </div>
            <div
              class=" col-md-6 col-lg-4 p-0   imageCover rounded-xl">
              <div class="gridinfo rounded-xl"></div>
            <!-- <img class="" src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/about-bride-540x405.jpg" alt="" srcset=""> -->
            </div>
            <div class="col-md-6 my-auto p-10 py-10 d-block d-md-none">
                <ProfileCard :aboutUs="bride"/>
              
            </div>
          </div>
      </div>
</template>

<script>
import ProfileCard from '../HomePageComp/ProfileCard.vue';
export default {
  components: { ProfileCard },
    name: 'WeddingAboutUs',

    data() {
        return {
            groom: {
              name: "William Adu",
            content: "Selassie is passionate about creating meaningful connections with people. He loves to explore, and share his experiences with others. With a keen eye for detail, Selassie takes pleasure in finding the beauty in the ordinary and transforming it into something extraordinary. On his wedding day, he is eager to celebrate love with his partner and share his joy with his loved ones.",
            cssClassContent: "text-lg-end",
            cssClassImage: "float-lg-end"
            },
            bride: {
              name: "Justine Diaba",
            content: "Delali is a beautiful soul who radiates joy wherever she goes. She has a heart of gold and a smile that can light up any room. Her love for life and adventure is contagious, and she is always up for trying something new. As she prepares to tie the knot, Delali is excited to start a new chapter with the love of her life 'Selassie' and create beautiful memories together.",
            cssClassContent: "text-start",
            cssClassImage: ""
            },
        };
    },

    mounted() {
        
    },

    methods: {
        
    },
};
</script>

<style scoped>

.brideGroomImage {
  background-image: url(https://res.cloudinary.com/dcyay2pow/image/upload/v1680936709/photos/WhatsApp_Image_2023-04-05_at_7.16.00_PM_nzmehp.jpg);
    height: 50vh;
    background-position: top top;
    background-repeat: no-repeat;
    background-size: cover;
    border: 0.1rem solid #b13a1a;
    border-radius: 5%;
    
}

.imageCover {
  background-image: url(https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/42631820_1066865700160854_8635461704899100672_n_ntkaxv.jpg);
    height: 50vh;
    background-position: top center;
    background-repeat: no-repeat;
    background-size: cover;
    border: 0.1rem solid #b13a1a;
    border-radius: 5%;
}

</style>