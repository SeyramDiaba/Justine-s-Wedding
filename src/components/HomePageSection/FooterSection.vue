<template>
    <div class="foot center">
        <img class="footerImage"
            src="https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/hero-logo.png"
            alt=""
          />
    </div>
</template>

<script>
export default {
    name: 'WeddingFooter',

    data() {
        return {
            
        };
    },

    mounted() {
        
    },

    methods: {
        
    },
};
</script>

<style  scoped>
.foot {
  position: absolute;
  /* top: 0px; */
  /* bottom: 0px; */
  width: 100%;
    height: 35rem;
    background-image: url(https://demo.singlestroke.io/jackrose/wp-content/uploads/2015/11/footer.jpg);
    background-repeat: no-repeat;
    background-size: cover;
  }

  .footerImage {
    height: 15rem;
  }
</style>