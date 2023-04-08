<template>
  <div id="whoWeAre" class="whoWeAre p-10  center bg-w boderAroundT" style="">
    
      <div class="row">
        <div class="col-md-5 mx-auto">
          <ProfileImage :whoarewe="groom"/>
          
        </div>
        <div class="col-md-2 py-xs-10 d-flex justify-content-center align-items-center">
          <img
            width="320"
            height="200"
            src="https://res.cloudinary.com/akwaah/image/upload/v1680436118/Untitled-1_mzqug3.png"
            alt=""
            loading="lazy"
          />
          

          <!-- <div class="H900 " style="font-size: 8rem; width:160;
            height:100;">
            &
          </div> -->
        </div>
        <div class="col-md-5">
          
          <ProfileImage :whoarewe="bride"/>
        </div>
 
      <div class="text-center mt-5">
        <p class="P400 N900" style="font-family: Alex Brush">Are getting married</p>
        <div class="P300 N900 mt-5">on 15th April, 2023 - Accra, Adenta</div>
      </div>
    </div>
  </div>
</template>

<script>
import ProfileImage from '../HomePageComp/ProfileImage.vue'
export default {
  components: { ProfileImage },
  name: 'WeddingWhoAreWe',

  data() {
    return {
      groom : {
          id: 1,
          name: "William Selasie Adu",
          photo: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680936709/photos/WhatsApp_Image_2023-04-05_at_7.16.00_PM_nzmehp.jpg"
        },
       bride: {
          id: 2,
          name: "Justine Delali Ama Diaba",
          photo: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680936265/photos/WhatsApp_Image_2023-04-05_at_7.50.09_PM_ol3hfu.jpg"
        }
      
    }
  },

  mounted() {},

  methods: {}
}
</script>

<style lang="scss" scoped></style>
