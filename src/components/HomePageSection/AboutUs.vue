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
            content: "Selasie is passionate about creating meaningful connections with people. He loves to explore, and share his experiences with others. With a keen eye for detail, Selasie takes pleasure in finding the beauty in the ordinary and transforming it into something extraordinary. On his wedding day, he is eager to celebrate love with his partner and share his joy with his loved ones.",
            cssClassContent: "text-lg-end",
            cssClassImage: "float-lg-end"
            },
            bride: {
              name: "Justine Diaba",
            content: "Justine is a beautiful soul who radiates joy wherever she goes. She has a heart of gold and a smile that can light up any room. Her love for life and adventure is contagious, and she is always up for trying something new. As she prepares to tie the knot, Justine is excited to start a new chapter with the love of her life 'Selasie' and create beautiful memories together.",
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
  background-image: url(https://cvws.icloud-content.com/B/AXaF1zbRh00eN6ypMtkk8KIwK16TAT9JtbjQVvhzh_Y6srkocmtGRQrI/profilepicsel.jpg?o=AkpI-8vT0SDGcjDmdZwcOr2kSGzcUVI1bnIpz1koJ_yQ&v=1&x=3&a=CAogzfHl8VcMKXri2rGGtGqESxozdttitQbiK80kWy14m6cSbxCC4o_M9zAYgr_rzfcwIgEAUgQwK16TWgRGRQrIaiegeMyJpBuAfOs7w0MX6Y7WyZwQXsXnEAHWmJH-RywGQvc2t6Y9R5tyJ1UPZMiCR1Q0pKijBVGcP31K1W19DwDOSQ447uVGyVDoHE-X1ZpT2g&e=1681374502&fl=&r=b76f973c-63ba-4815-aac4-4230d7a442e2-1&k=cbuKpOBR1LYqxwE_ylwJpA&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=g4cW_hp3e-H0OsfpUM7hGym_RqM&cd=i);
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