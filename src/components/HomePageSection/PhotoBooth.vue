<template>
  <div id="gallery ">
    <div class="text-center H900 N600 my-10">Gallery</div>
    <div class="row ">
      <div class="column ">
        <img src="https://cvws.icloud-content.com/B/AQvtxKZEJf59jG0Kg3eZf9doPR0-AU2EYsvBLmG_GufORnDxZSS4JRk4/WJ-PW-6.JPG?o=AjFUsvDmhYfPgPWNFf6QrzbYY_N_LP439jkhbAB7BKeL&v=1&x=3&a=CAogELSqiEIHjobmTIAJJBaxjOkEU4MkEMpE_DYX73rWWisSbxCUir7I9zAYlOeZyvcwIgEAUgRoPR0-WgS4JRk4aiedpkpX0abzyLLA2dwQOCg5-ttaJMw6SN2n1lCvOIBhAwav46UEzCByJ5J-FNbJDP7t-jEif41J-H_AT74LwlQzwVR4FpiADQ9oTBjeUq82sw&e=1681366872&fl=&r=0ae065d2-80b5-4c0a-9baa-db4e36968c1a-1&k=K97epFfAyztxVM9uJN7T0w&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=8ixjZL990qXiiMaCMIlf3IHxjJY&cd=i" @click="openModal(1)" class="hover-shadow rounded-xl ">
        <img src="https://res.cloudinary.com/dcyay2pow/image/upload/v1680935529/photos/WhatsApp_Image_2023-04-05_at_7.11.50_PM_p1zr1y.jpg" @click="openModal(2)" class="hover-shadow rounded-xl">
        <img src="https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/WhatsApp_Image_2023-04-05_at_7.37.48_PM_xx5ia1.jpg" @click="openModal(3)" class="hover-shadow rounded-xl">
      </div>
      <div class="column">
        <img src="https://cvws.icloud-content.com/B/AYJE10n76OYPhsU8IdlEoLxbeutQASTWVjdVbmGeWWsusQQ0EQT6VI2C/WJ-PW-5.JPG?o=AicrqWlapOaXKPMm5imQgCLi7fz5bi4Ueixb6d3Lg8Cl&v=1&x=3&a=CAog665EPgjC4dFz4K0kdTwORf0UkOH4DQox7lE-CE_0SxQSbxCLir7I9zAYi-eZyvcwIgEAUgRbeutQWgT6VI2Caic9Ny9mhA8ZUGjDhupsOeFClf1lzD_h5xOoVKVJxO-42cU8wIAxAElyJ9tFCPzR65KCvK-h8j9Smin14Q_Lv0tNIzpm9DuURqsaoSc3aNvhbw&e=1681366872&fl=&r=0ae065d2-80b5-4c0a-9baa-db4e36968c1a-1&k=1cBcS1eswxTwcbpzgGdnfw&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=meou-PpRZ1AFm8xEGeTJVUhL0C0&cd=i" @click="openModal(4)" class="hover-shadow rounded-xl">
        <img src="https://res.cloudinary.com/dcyay2pow/image/upload/v1680935534/photos/WhatsApp_Image_2023-04-05_at_8.27.45_PM_bn3pzy.jpg" @click="openModal(5)" class="hover-shadow rounded-xl">
        <!-- <img src="https://res.cloudinary.com/akwaah/image/upload/v1680378377/IMG_20220219_124010_ibtdcs.jpg" @click="openModal(6)" class="hover-shadow rounded-xl"> -->
        
      </div>
      <div class="column">
        <img src="https://cvws.icloud-content.com/B/AZ0engJVXW3tMytAddoeG0R7hjcuASZOwoi2F-lZ9no4lWb6ul7kEW0S/WJ-PW-2.JPG?o=AnumQAPhC80XHlgdAeto2Vks834rnWCVv00eii9r4Tg2&v=1&x=3&a=CAog2wOYWkd8vw1FQJ7cqFO9EXQROi20r_1TAcazeTVeDFsSbxCixMHI9zAYoqGdyvcwIgEAUgR7hjcuWgTkEW0SaifChqXzcCk-2tGHxRIJ7RA8xQ9EOGyttY0OwKz0C6ndhl8g7Wa0g3VyJ8I_6SWGnaNtF33eN4FYXlQ_RBHiQiVjGvuPR58hzdJHjhLa6kViAw&e=1681366929&fl=&r=f02a1dc2-37ac-4ffc-a08a-9c49a5b4b813-1&k=cWL4ds_VqIu7fjh6eA9KyA&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=Jh8ZIo2hsB5oWW0GR7_zvpMjodE&cd=i" @click="openModal(7)" class="hover-shadow rounded-xl">
        <img src="https://cvws.icloud-content.com/B/ARrwYhvOFlMov8fQ-9BfHIzDZvzfAVOit9R0bg3a-hq10HyUNeH9Y2Gk/WJ-PW-1.JPG?o=AoUgnJNdcikk93ckBEuN6LT1Cch4rFNT4RE3RadEAjpv&v=1&x=3&a=CAogA01PfbbWgqvIVvh77XZT6rHVwrUpugwEoNhVnd055QoSbxCtjcHI9zAYreqcyvcwIgEAUgTDZvzfWgT9Y2GkaidBwBZGav-cl2C7Q6MlDYbQi7IU25TJ6c9I-WeinLdg10E_ATt5JgRyJzepeVNLWdRLNPm6xNUkMe1oa3CDbQtxRSPsy3LRFd1IaUMSMS3qHg&e=1681366922&fl=&r=50a23980-2488-436f-9a57-aec522aef1dc-1&k=d1vJT-WicwtQFTWnIEzmmg&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=WvBuhgSzi6mpZ6fqiI2oGx6Zrlo&cd=i" @click="openModal(8)" class="hover-shadow rounded-xl">
        <!-- <img src="https://res.cloudinary.com/akwaah/image/upload/v1680380208/IMG_20220219_133542_1_x5b2ds.jpg" @click="openModal(9)" class="hover-shadow rounded-xl"> -->
        <!-- <img src="https://res.cloudinary.com/akwaah/image/upload/v1680380196/IMG_20220430_131627_nduefu.jpg" @click="openModal(10)" class="hover-shadow rounded-xl"> -->
      </div>
      <div class="column">
        <img src="https://cvws.icloud-content.com/B/AXN33ckIvvLRqBiz7rh5YJcbcHjIAYEPOgf7I3G3LfODbbY_VhZ6KcTh/red+carpet+2.jpg?o=AqRqfZYC7qsZFhghpsm6toVy4HXV5Qm8658JhGhdoNa_&v=1&x=3&a=CAogme4rcdX6KzB1kcPGP0Si-fK22kkMYij__4Zj4TPHVusSbxDT2b_I9zAY07abyvcwIgEAUgQbcHjIWgR6KcThaid8biS25g-t4wS-YECcLv4MP-3h7WPx5Op-4gsN0r7mmTY2EWG5u6hyJwMBE0ECGzNlv_cAsEJyUUb8kB9RYyQyHxo9o0KYlwDjPnBiMBiAmw&e=1681366899&fl=&r=cd4293ea-9f82-4203-a9b7-94934f732463-1&k=Fz5EB1dwqeDBVwIJz9Va3w&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=9_gUEhxpmxWXbi3HX-OCmsEmoWU&cd=i" @click="openModal(11)" class="hover-shadow rounded-xl">
        <!-- <img src="https://cvws.icloud-content.com/B/AVdKMArDtv9_hEnfm-x8Ghup4DECAXvAWtXKx5tNcslnh1_ZlRsIIIWV/WhatsApp+Image+2023-04-08+at+1.22.16+PM.jpeg?o=AqEykrsA1TU7y0SsU3bKaLEm0kKZVPeMLTUc7mCtEydl&v=1&x=3&a=CAogblmvWv4VxSyvwBl_npq1oXQjT48p0tP_w6LUQkJkuuESbxCQ8MDI9zAYkM2cyvcwIgEAUgSp4DECWgQIIIWVaifp6sMlgOfxrA6mLWIzVmUzOREbxxP5CvRA9Y61nCyGXIf_KyoLrRZyJ2r8FFsLCg3INRbIiVL71Ma73lcUCrW_MQVREsAfurcEnEjO2kRz9g&e=1681366918&fl=&r=137191a9-da92-417e-9b29-360f9dfc5548-1&k=5r7w5PzNvHDsWv91e7B-Aw&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=hXq3FlO_5YKX9NylNA1SpbPlCr0&cd=i" @click="openModal(12)" class="hover-shadow rounded-xl"> -->
        <!-- <img src="https://res.cloudinary.com/akwaah/image/upload/v1680380165/IMG_20220219_121336_pp0xmv.jpg" @click="openModal(13)" class="hover-shadow rounded-xl"> -->
      </div>
     
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
        { src: "https://cvws.icloud-content.com/B/AQvtxKZEJf59jG0Kg3eZf9doPR0-AU2EYsvBLmG_GufORnDxZSS4JRk4/WJ-PW-6.JPG?o=AjFUsvDmhYfPgPWNFf6QrzbYY_N_LP439jkhbAB7BKeL&v=1&x=3&a=CAogELSqiEIHjobmTIAJJBaxjOkEU4MkEMpE_DYX73rWWisSbxCUir7I9zAYlOeZyvcwIgEAUgRoPR0-WgS4JRk4aiedpkpX0abzyLLA2dwQOCg5-ttaJMw6SN2n1lCvOIBhAwav46UEzCByJ5J-FNbJDP7t-jEif41J-H_AT74LwlQzwVR4FpiADQ9oTBjeUq82sw&e=1681366872&fl=&r=0ae065d2-80b5-4c0a-9baa-db4e36968c1a-1&k=K97epFfAyztxVM9uJN7T0w&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=8ixjZL990qXiiMaCMIlf3IHxjJY&cd=i", wideSrc: "https://cvws.icloud-content.com/B/AQvtxKZEJf59jG0Kg3eZf9doPR0-AU2EYsvBLmG_GufORnDxZSS4JRk4/WJ-PW-6.JPG?o=AjFUsvDmhYfPgPWNFf6QrzbYY_N_LP439jkhbAB7BKeL&v=1&x=3&a=CAogELSqiEIHjobmTIAJJBaxjOkEU4MkEMpE_DYX73rWWisSbxCUir7I9zAYlOeZyvcwIgEAUgRoPR0-WgS4JRk4aiedpkpX0abzyLLA2dwQOCg5-ttaJMw6SN2n1lCvOIBhAwav46UEzCByJ5J-FNbJDP7t-jEif41J-H_AT74LwlQzwVR4FpiADQ9oTBjeUq82sw&e=1681366872&fl=&r=0ae065d2-80b5-4c0a-9baa-db4e36968c1a-1&k=K97epFfAyztxVM9uJN7T0w&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=8ixjZL990qXiiMaCMIlf3IHxjJY&cd=i", alt: "Nature" },
        { src: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935529/photos/WhatsApp_Image_2023-04-05_at_7.11.50_PM_p1zr1y.jpg", wideSrc: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/WhatsApp_Image_2023-04-05_at_7.37.48_PM_xx5ia1.jpg", alt: "Snow" },
        { src: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/WhatsApp_Image_2023-04-05_at_7.37.48_PM_xx5ia1.jpg", wideSrc: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935533/photos/WhatsApp_Image_2023-04-05_at_7.37.48_PM_xx5ia1.jpg", alt: "Mountains" },
        
        { src: "https://cvws.icloud-content.com/B/AYJE10n76OYPhsU8IdlEoLxbeutQASTWVjdVbmGeWWsusQQ0EQT6VI2C/WJ-PW-5.JPG?o=AicrqWlapOaXKPMm5imQgCLi7fz5bi4Ueixb6d3Lg8Cl&v=1&x=3&a=CAog665EPgjC4dFz4K0kdTwORf0UkOH4DQox7lE-CE_0SxQSbxCLir7I9zAYi-eZyvcwIgEAUgRbeutQWgT6VI2Caic9Ny9mhA8ZUGjDhupsOeFClf1lzD_h5xOoVKVJxO-42cU8wIAxAElyJ9tFCPzR65KCvK-h8j9Smin14Q_Lv0tNIzpm9DuURqsaoSc3aNvhbw&e=1681366872&fl=&r=0ae065d2-80b5-4c0a-9baa-db4e36968c1a-1&k=1cBcS1eswxTwcbpzgGdnfw&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=meou-PpRZ1AFm8xEGeTJVUhL0C0&cd=i", wideSrc: "https://cvws.icloud-content.com/B/AYJE10n76OYPhsU8IdlEoLxbeutQASTWVjdVbmGeWWsusQQ0EQT6VI2C/WJ-PW-5.JPG?o=AicrqWlapOaXKPMm5imQgCLi7fz5bi4Ueixb6d3Lg8Cl&v=1&x=3&a=CAog665EPgjC4dFz4K0kdTwORf0UkOH4DQox7lE-CE_0SxQSbxCLir7I9zAYi-eZyvcwIgEAUgRbeutQWgT6VI2Caic9Ny9mhA8ZUGjDhupsOeFClf1lzD_h5xOoVKVJxO-42cU8wIAxAElyJ9tFCPzR65KCvK-h8j9Smin14Q_Lv0tNIzpm9DuURqsaoSc3aNvhbw&e=1681366872&fl=&r=0ae065d2-80b5-4c0a-9baa-db4e36968c1a-1&k=1cBcS1eswxTwcbpzgGdnfw&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=meou-PpRZ1AFm8xEGeTJVUhL0C0&cd=i", alt: "Lights" },
        { src: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935534/photos/WhatsApp_Image_2023-04-05_at_8.27.45_PM_bn3pzy.jpg", wideSrc: "https://res.cloudinary.com/dcyay2pow/image/upload/v1680935534/photos/WhatsApp_Image_2023-04-05_at_8.27.45_PM_bn3pzy.jpg", alt: "Snow" },
        // { src: "https://res.cloudinary.com/akwaah/image/upload/v1680378377/IMG_20220219_124010_ibtdcs.jpg", wideSrc: "https://res.cloudinary.com/akwaah/image/upload/v1680203747/CG7A3084_ihsozw.jpg", alt: "Mountains" },
        
         { src: "https://cvws.icloud-content.com/B/AZ0engJVXW3tMytAddoeG0R7hjcuASZOwoi2F-lZ9no4lWb6ul7kEW0S/WJ-PW-2.JPG?o=AnumQAPhC80XHlgdAeto2Vks834rnWCVv00eii9r4Tg2&v=1&x=3&a=CAog2wOYWkd8vw1FQJ7cqFO9EXQROi20r_1TAcazeTVeDFsSbxCixMHI9zAYoqGdyvcwIgEAUgR7hjcuWgTkEW0SaifChqXzcCk-2tGHxRIJ7RA8xQ9EOGyttY0OwKz0C6ndhl8g7Wa0g3VyJ8I_6SWGnaNtF33eN4FYXlQ_RBHiQiVjGvuPR58hzdJHjhLa6kViAw&e=1681366929&fl=&r=f02a1dc2-37ac-4ffc-a08a-9c49a5b4b813-1&k=cWL4ds_VqIu7fjh6eA9KyA&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=Jh8ZIo2hsB5oWW0GR7_zvpMjodE&cd=i", wideSrc: "https://cvws.icloud-content.com/B/AZ0engJVXW3tMytAddoeG0R7hjcuASZOwoi2F-lZ9no4lWb6ul7kEW0S/WJ-PW-2.JPG?o=AnumQAPhC80XHlgdAeto2Vks834rnWCVv00eii9r4Tg2&v=1&x=3&a=CAog2wOYWkd8vw1FQJ7cqFO9EXQROi20r_1TAcazeTVeDFsSbxCixMHI9zAYoqGdyvcwIgEAUgR7hjcuWgTkEW0SaifChqXzcCk-2tGHxRIJ7RA8xQ9EOGyttY0OwKz0C6ndhl8g7Wa0g3VyJ8I_6SWGnaNtF33eN4FYXlQ_RBHiQiVjGvuPR58hzdJHjhLa6kViAw&e=1681366929&fl=&r=f02a1dc2-37ac-4ffc-a08a-9c49a5b4b813-1&k=cWL4ds_VqIu7fjh6eA9KyA&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=Jh8ZIo2hsB5oWW0GR7_zvpMjodE&cd=i", alt: "Lights" },
         { src: "https://cvws.icloud-content.com/B/ARrwYhvOFlMov8fQ-9BfHIzDZvzfAVOit9R0bg3a-hq10HyUNeH9Y2Gk/WJ-PW-1.JPG?o=AoUgnJNdcikk93ckBEuN6LT1Cch4rFNT4RE3RadEAjpv&v=1&x=3&a=CAogA01PfbbWgqvIVvh77XZT6rHVwrUpugwEoNhVnd055QoSbxCtjcHI9zAYreqcyvcwIgEAUgTDZvzfWgT9Y2GkaidBwBZGav-cl2C7Q6MlDYbQi7IU25TJ6c9I-WeinLdg10E_ATt5JgRyJzepeVNLWdRLNPm6xNUkMe1oa3CDbQtxRSPsy3LRFd1IaUMSMS3qHg&e=1681366922&fl=&r=50a23980-2488-436f-9a57-aec522aef1dc-1&k=d1vJT-WicwtQFTWnIEzmmg&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=WvBuhgSzi6mpZ6fqiI2oGx6Zrlo&cd=i", wideSrc: "https://cvws.icloud-content.com/B/ARrwYhvOFlMov8fQ-9BfHIzDZvzfAVOit9R0bg3a-hq10HyUNeH9Y2Gk/WJ-PW-1.JPG?o=AoUgnJNdcikk93ckBEuN6LT1Cch4rFNT4RE3RadEAjpv&v=1&x=3&a=CAogA01PfbbWgqvIVvh77XZT6rHVwrUpugwEoNhVnd055QoSbxCtjcHI9zAYreqcyvcwIgEAUgTDZvzfWgT9Y2GkaidBwBZGav-cl2C7Q6MlDYbQi7IU25TJ6c9I-WeinLdg10E_ATt5JgRyJzepeVNLWdRLNPm6xNUkMe1oa3CDbQtxRSPsy3LRFd1IaUMSMS3qHg&e=1681366922&fl=&r=50a23980-2488-436f-9a57-aec522aef1dc-1&k=d1vJT-WicwtQFTWnIEzmmg&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=WvBuhgSzi6mpZ6fqiI2oGx6Zrlo&cd=i", alt: "Snow" },
        // { src: "https://res.cloudinary.com/akwaah/image/upload/v1680380208/IMG_20220219_133542_1_x5b2ds.jpg", wideSrc: "https://res.cloudinary.com/akwaah/image/upload/v1680203747/CG7A3084_ihsozw.jpg", alt: "Mountains" },
        // { src: "https://res.cloudinary.com/akwaah/image/upload/v1680380196/IMG_20220430_131627_nduefu.jpg", wideSrc: "https://res.cloudinary.com/akwaah/image/upload/v1680203721/CG7A3085_v2kbeh.jpg", alt: "Lights" },

         { src: "https://cvws.icloud-content.com/B/AXN33ckIvvLRqBiz7rh5YJcbcHjIAYEPOgf7I3G3LfODbbY_VhZ6KcTh/red+carpet+2.jpg?o=AqRqfZYC7qsZFhghpsm6toVy4HXV5Qm8658JhGhdoNa_&v=1&x=3&a=CAogme4rcdX6KzB1kcPGP0Si-fK22kkMYij__4Zj4TPHVusSbxDT2b_I9zAY07abyvcwIgEAUgQbcHjIWgR6KcThaid8biS25g-t4wS-YECcLv4MP-3h7WPx5Op-4gsN0r7mmTY2EWG5u6hyJwMBE0ECGzNlv_cAsEJyUUb8kB9RYyQyHxo9o0KYlwDjPnBiMBiAmw&e=1681366899&fl=&r=cd4293ea-9f82-4203-a9b7-94934f732463-1&k=Fz5EB1dwqeDBVwIJz9Va3w&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=9_gUEhxpmxWXbi3HX-OCmsEmoWU&cd=i", wideSrc: "https://cvws.icloud-content.com/B/AXN33ckIvvLRqBiz7rh5YJcbcHjIAYEPOgf7I3G3LfODbbY_VhZ6KcTh/red+carpet+2.jpg?o=AqRqfZYC7qsZFhghpsm6toVy4HXV5Qm8658JhGhdoNa_&v=1&x=3&a=CAogme4rcdX6KzB1kcPGP0Si-fK22kkMYij__4Zj4TPHVusSbxDT2b_I9zAY07abyvcwIgEAUgQbcHjIWgR6KcThaid8biS25g-t4wS-YECcLv4MP-3h7WPx5Op-4gsN0r7mmTY2EWG5u6hyJwMBE0ECGzNlv_cAsEJyUUb8kB9RYyQyHxo9o0KYlwDjPnBiMBiAmw&e=1681366899&fl=&r=cd4293ea-9f82-4203-a9b7-94934f732463-1&k=Fz5EB1dwqeDBVwIJz9Va3w&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=9_gUEhxpmxWXbi3HX-OCmsEmoWU&cd=i", alt: "Snow" },
        //  { src: "https://cvws.icloud-content.com/B/AVdKMArDtv9_hEnfm-x8Ghup4DECAXvAWtXKx5tNcslnh1_ZlRsIIIWV/WhatsApp+Image+2023-04-08+at+1.22.16+PM.jpeg?o=AqEykrsA1TU7y0SsU3bKaLEm0kKZVPeMLTUc7mCtEydl&v=1&x=3&a=CAogblmvWv4VxSyvwBl_npq1oXQjT48p0tP_w6LUQkJkuuESbxCQ8MDI9zAYkM2cyvcwIgEAUgSp4DECWgQIIIWVaifp6sMlgOfxrA6mLWIzVmUzOREbxxP5CvRA9Y61nCyGXIf_KyoLrRZyJ2r8FFsLCg3INRbIiVL71Ma73lcUCrW_MQVREsAfurcEnEjO2kRz9g&e=1681366918&fl=&r=137191a9-da92-417e-9b29-360f9dfc5548-1&k=5r7w5PzNvHDsWv91e7B-Aw&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=hXq3FlO_5YKX9NylNA1SpbPlCr0&cd=i", wideSrc: "https://cvws.icloud-content.com/B/AVdKMArDtv9_hEnfm-x8Ghup4DECAXvAWtXKx5tNcslnh1_ZlRsIIIWV/WhatsApp+Image+2023-04-08+at+1.22.16+PM.jpeg?o=AqEykrsA1TU7y0SsU3bKaLEm0kKZVPeMLTUc7mCtEydl&v=1&x=3&a=CAogblmvWv4VxSyvwBl_npq1oXQjT48p0tP_w6LUQkJkuuESbxCQ8MDI9zAYkM2cyvcwIgEAUgSp4DECWgQIIIWVaifp6sMlgOfxrA6mLWIzVmUzOREbxxP5CvRA9Y61nCyGXIf_KyoLrRZyJ2r8FFsLCg3INRbIiVL71Ma73lcUCrW_MQVREsAfurcEnEjO2kRz9g&e=1681366918&fl=&r=137191a9-da92-417e-9b29-360f9dfc5548-1&k=5r7w5PzNvHDsWv91e7B-Aw&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=59&s=hXq3FlO_5YKX9NylNA1SpbPlCr0&cd=i", alt: "Mountains" },
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
