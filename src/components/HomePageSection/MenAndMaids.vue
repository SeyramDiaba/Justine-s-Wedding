<template>
    <div>
        <div class="menAndMaids p-10 container">
            <div class="text-center P400 N600 mb-10">The Groomsmen</div>

            <div class=" d-none d-md-block">
            <div class="hstack gap-3">
                <ProfileImage/>
                <ProfileImage/>
                <ProfileImage/>
                <ProfileImage/>
                <ProfileImage/>
                <ProfileImage/>
            </div>
        </div>
        <div class=" d-block d-md-none">
            <div class="vstack gap-3 ">
                <ProfileImage/>
                <ProfileImage/>
                <ProfileImage/>
                <ProfileImage/>
                <ProfileImage/>
                <ProfileImage/>
            </div>
        </div>
        </div>
    </div>
</template>

<script>
import ProfileImage from '../HomePageComp/ProfileImage.vue';

export default {
    name: "WeddingMenAndMaids",
    data() {
        return {};
    },
    mounted() {
    },
    methods: {},
    components: { ProfileImage }
};
</script>

<style lang="scss" scoped>

</style>