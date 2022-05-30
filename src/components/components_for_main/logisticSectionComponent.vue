<template>
    <section id="logistic-services">
        <div class="container h-100">
            <div class="row row-cols-3 h-100 d-flex align-items-center">
                
                <div class="col">
                    <div class="my_card p-5 h-100">
                        <img class="w-100 " src="../../assets/img/gallery-3.jpg" alt="">
                        <div class="text h-50">
                            <h3 class="my-2">Tecnology</h3>
                            <p>Focused on developing technology solutions adapted to our client's needs.</p>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="my_card p-5 h-100">
                        <img class="w-100 " src="../../assets/img/gallery-3.jpg" alt="">
                        <div class="text h-50">
                            <h3 class="my-4">Tecnology</h3>
                            <p>Focused on developing technology solutions adapted to our client's needs.</p>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="my_card p-5 h-100">
                        <img class="w-100 " src="../../assets/img/gallery-5.jpg" alt="">
                        <div class="text h-50">
                            <h3 class="my-4">Transport</h3>
                            <p>We develop operational strategies to improve logistical efficiency.</p>
                        </div>
                    </div>
                </div>
                
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'logisticSectionComponent',
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/vars';

    section{
        height: 600px;
        background-color: $colorCube_saltpan;

        .col{ 
            width: 30%;
        }
    }

    .my_card{ 
        border-radius: 15px;
        background-color: white;
    }
</style>