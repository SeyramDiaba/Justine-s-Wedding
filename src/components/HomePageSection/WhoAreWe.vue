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
          name: "William Adu",
          photo: "https://cvws.icloud-content.com/B/AXaF1zbRh00eN6ypMtkk8KIwK16TAT9JtbjQVvhzh_Y6srkocmtGRQrI/profilepicsel.jpg?o=Amx7WRpKmhrzwp1CVmBxsJYaMMEYtslPi5u2caIwr2ZZ&v=1&x=3&a=CAogZ2G_X2fd2r4QOnbTDwfZpF3UD-YFa6l3lsnUAWXbCnISbxC2_afJ9zAYttqDy_cwIgEAUgQwK16TWgRGRQrIaic012umuonA68WQdJySe5Pb3931fgkuem2f9fFjdjLUGGzl4CrHjU1yJ9ShAorrWIKZk1yzkdLIqExsZh1gXTecFn7VHtvPaprOhNmRjo3fMg&e=1681368608&fl=&r=b96e6487-7381-459f-99de-57ec8a16ec2d-1&k=cbuKpOBR1LYqxwE_ylwJpA&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=QwE8rQK7kPB0YaJOIdSzW2-tSBk&cd=i"
        },
       bride: {
          id: 2,
          name: "Justine Diaba",
          photo: "https://cvws.icloud-content.com/B/AYrH_iZvjz391GTUfPip91_sEScXAUJRMwY-XcC4_kSqpkHICQgcwf6v/justineprofile.jpg?o=Amq9oUE3tCU0MC_Pfl0URRwl7R6g5AcoYMX4xJKNQklL&v=1&x=3&a=CAogX5LfSDKZOHBrChDiGFnSMsWRiicsTgt3VvA8M-y16GUSbxDYs7bJ9zAY2JCSy_cwIgEAUgTsEScXWgQcwf6vaieTyARiC2FS-XxLePZOIKHAtHJTkcxZcrP8f9Us2lXTqbX5sEoLdUhyJ8r124EQ5IcIwlL146aGD8ZGaypapYZDMJ_9YBxpwMqOAfoc1dBMmg&e=1681368844&fl=&r=0e8ffb59-096c-4b57-9c5b-d31457e6a0d2-1&k=o0eDgK1IKOwOqUsrNpOuSA&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=nM12jBWeswXOfm8ysUfpAMZYRVQ&cd=i"
        }
      
    }
  },

  mounted() {},

  methods: {}
}
</script>

<style lang="scss" scoped></style>
