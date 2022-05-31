<template>
  <section id="partners">
    <div class="container h-100">
        <div class="h-100 row row-cols-6 d-flex justify-content-between align-items-center">
            <div class="col">
                <img class="rounded mx-auto d-block" src="../../assets/img/logo-1.png" alt="">
            </div>
            <div class="col">
                <img class="rounded mx-auto d-block" src="../../assets/img/logo-2.png" alt="">
            </div>
            <div class="col">
                <img class="rounded mx-auto d-block" src="../../assets/img/logo-3.png" alt="">
            </div>
            <div class="col">
                <img class="rounded mx-auto d-block" src="../../assets/img/logo-4.png" alt="">
            </div>
            <div class="col">
                <img class="rounded mx-auto d-block" src="../../assets/img/logo-5.png" alt="">
            </div>
            <div class="col">
                <img class="rounded mx-auto d-block" src="../../assets/img/logo-1.png" alt="">
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'partnersSectionComponent'
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