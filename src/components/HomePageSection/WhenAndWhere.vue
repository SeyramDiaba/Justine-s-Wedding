<template>
    <div class="bgColor2">
    <div id="whenNwhere" class="whenNwhere p-10 container ">
          <div class="text-center H900 N600 mb-10">When & Where</div>
          <div class="row g-3">
            <div class="col-md-6 col-12 pl-0 ">
              <div class=" justify-content-center">
                <!-- <img
                  src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/event-party-540x270.jpg"
                  alt=""
                /> -->
                <div class="center avatar borderColor  mx-auto rounded-circle" style="background: #d0edf5; ">
                  <Engagement/>
                </div>
                <div class="p-lg-10 p-5                      
                 text-center">
                  <div class="P400 N900 py-2 text-capitalize">Engagement</div>
                  <div class="P200 N900 py-2 text-capitalize">
                    Friday, 14 April
                  </div>
                  <div class="P200 N900 py-2 text-capitalize">
                    8.00 AM
                  </div>
                  <div class="P200 N900 py-2 text-capitalize">
                    Mr. Diaba Thaddeus' Residence
                  </div>
                  <div class="P200 N900 py-2 text-capitalize">
                    Adenta-Frafraha, Greater Accra Region
                  </div>
                  <div class="P200 N900 py-2 text-capitalize" style="color: #b13a1a">
                    RSVP: Stephen Diaba<br>Tel: 0500190679
                  </div>
                  <a  href="https://goo.gl/maps/LzmsXBfnSLgKk4Ak8" target="_blank" type="button" class="btn bgColor2 borderColor py-2 text-capitalize" style="color: #b13a1a">View map</a>
                </div>
              </div>
            </div>

            <div class="col-md-6 col-12 pr-0">
              <div class=" justify-content-center">
                <div class="center avatar borderColor  mx-auto rounded-circle" style="background: #d0edf5; ">
                  <Church/>
                </div>
                <div class="p-lg-10 p-5                      
                 text-center">
                  <div class="P400 N900 py-2 text-capitalize">Wedding</div>
                  <div class="P200 N900 py-2 text-capitalize">
                    Saturday, 15 April
                  </div>
                  <div class="P200 N900 py-2 text-capitalize">
                    11.00 AM
                  </div>
                  <div class="P200 N900 py-2 text-capitalize">
                    St. John The Evangelist Catholic Church
                  </div>
                  <div class="P200 N900 py-2 text-capitalize">
                    Adenta, Greater Accra Region
                  </div>
                  <div class="P200 N900 py-2 text-capitalize" style="color: #b13a1a">
                    RSVP: Stephen Diaba<br>Tel: 0500190679
                  </div>
                  <a  href="https://goo.gl/maps/pGXYe4Ge8x7NJmhU9" target="_blank" type="button" class="btn bgColor2 borderColor py-2 text-capitalize" style="color: #b13a1a">View map</a>
                </div>
              </div>
              
            </div>
          </div>
          
      </div>
      <!-- map -->
      <div id="map" class="map  center bgColor boderAroundT">
            <!-- <iframe v-if="this.showEngagementLoc" src="ttps://www.google.com/maps/embed?pb=!1m17!1m12!1m3!1d3969.852352506723!2d-0.14890100000000003!3d5.734394!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m2!1m1!2zNcKwNDQnMDMuOCJOIDDCsDA4JzU2LjAiVw!5e0!3m2!1sen!2sgh!4v1680935040832!5m2!1sen!2sghh" width="10000rem" height="600" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe> -->
            <iframe v-if="true" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3969.9961184216436!2d-0.1550639851247383!3d5.713694122348918!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xfdf9d6049054b2d%3A0xede88d57e8610474!2sSt%20John%20the%20Evangelist%20Catholic%20Church!5e0!3m2!1sen!2sgh!4v1681075280351!5m2!1sen!2sgh" width="100%" height="600" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
    </div>
</template>

<script>
import Church from '../icons/church.vue';
import church from '../icons/church.vue';
import Engagement from '../icons/engagement.vue';
export default {
  components: { church, Church, Engagement },
    name: 'WeddingWhenAndHere',

    data() {
        return {
          showEngagementLoc: '',
          showWeddingLoc: ''
        };
    },

    mounted() {
        
    },

    methods: {
    setWeddingLoc ( wedding, engagement) { 
      showWeddingLoc = wedding
      showEngagementLoc = engagement
    },
    setEngagementLoc () {
      showEngagementLoc = true
      showWeddingLoc = false
    },
        
    },
    computed: {
      
    }
};
</script>

<style scoped>
.avatar {
        width: 10rem;
        height: 10rem;
        
      }
</style>