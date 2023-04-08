<template>
  <div class="">
    <img
      class="avatar mx-auto rounded-circle borderColor"
      :src='whoarewe.photo'
      alt="Rounded avatar"
    />
    <div class="P300 N900 text-center mt-5">{{ whoarewe.name }}</div>
  </div>
</template>

<script>
export default {
  props: {
   whoarewe: {
    id: Number,
    photo: String,
    name: String
   },
   
  },
  name: 'WeddingProfileImage',

  data() {
    return {}
  },

  mounted() {},

  methods: {}
}
</script>

<style scoped>

</style>
