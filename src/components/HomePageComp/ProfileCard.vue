<template>
    <div class="">
        <div class="P400 N900 py-5 " :class="aboutUs.cssClassContent" >{{aboutUs.name}}</div>
              <div class="P200 N900  " :class="aboutUs.cssClassContent">
                {{ aboutUs.content }}
              </div>
        <div class="" :class="aboutUs.cssClassImage" >
            <!-- <img src="../../assets/2950180.png" alt="" srcset=""> -->
            <Dove/>
        </div>
    </div>
</template>

<script>
import Dove from '../icons/dove.vue';

export default {
  props: {
    aboutUs: {
        name: String,
        content: String,
        cssClassContent: String,
        cssClassImage: String
    }
  },
    name: "ProfileCard",
    data() {
        return {};
    },
    mounted() {
    },
    methods: {},
    components: { Dove }
};
</script>

<style lang="scss" scoped>

</style>