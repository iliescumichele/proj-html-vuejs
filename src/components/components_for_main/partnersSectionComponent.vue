<template>
  <section id="partners">
    <div class="container h-100">
        <div class="h-100 row row-cols-6 d-flex justify-content-between align-items-center">
            <div class="col"
                v-for="(url,index) in partnersImgList"
                :key="`url${index}`"
            >
                <img class="rounded mx-auto d-block" :src="getImgUrl(url)" alt="">
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'partnersSectionComponent',

    data(){
        return{
            partnersImgList: [
                "logo-1.png",
                "logo-2.png",
                "logo-3.png",
                "logo-4.png",
                "logo-5.png",
                "logo-1.png"
            ]
        }
    },

    methods:{
        getImgUrl(thumb){
            return require('../../assets/img/' + thumb)
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/vars';

    section{ 
        height: 300px;
        background-color: $colorCube_saltpan;

        img{
            width: 50%;
            color: $colorCube_manatee;
            opacity: .6;
        }
    }
</style>