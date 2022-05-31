<template>
    <section id="services">
        <div class="container h-100">
            <div class="row row-cols-3 h-100 d-flex align-items-center">
                <div class="col ">
                    <div class="text-logistic-services h-100">
                        <h4>OUR BUSINESS AREAS</h4>
                        <h2 class="my-4">Logistics Services</h2>
                        <p class="my-4">We are leaders in providing logistics services with a set of cutting edge tecnologies and a team of experienced and renowned professionals.</p>
                    </div>
                    <div class="qualities">
                        <div class="btn-general">Tradition</div>
                        <div class="btn-general">Quality</div>
                        <div class="btn-general">Security</div>
                    </div>
                    <button type="button" class="btn my-4">READ MORE</button> 
                </div>
                <div class="col">
                    <div class="my_card p-5 h-100">
                        <img class="w-100 " src="../../assets/img/gallery-3.jpg" alt="">
                        <div class="text ">
                            <h3 class="my-4">Tecnology</h3>
                            <p>Focused on developing technology solutions adapted to our client's needs.</p>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="my_card p-5 h-100">
                        <img class="w-100 " src="../../assets/img/gallery-5.jpg" alt="">
                        <div class="text">
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
        height: 700px;
        background-color: $colorCube_saltpan;

        .col{ 
            width: 30%;
            margin: auto 10px;
            p{ 
                font-size: 1.15rem;
                color: $colorCube_manatee;
            }
        }
    }

    .text-logistic-services{
        h4{ 
            font-size: 0.9rem;
            font-weight: 800;
            color: $materialDesign_elfGreen;
        }
        
        h2{
            font-size: 3rem;
            font-weight: 800;
            color: $medinCut_outerSpace;
        }

    }

    .qualities{ 
        .btn-general{
            display: inline-block;
            color: $colorCube_blueLagoon;
            background-color: $colorCube_blueLagoonAlpha;
            margin-right: 15px;
            margin-left: 0;
        }
    }

    .btn{ 
        background-color: $colorCube_blueLagoon;
        color: $medinCut_grayNurse;
        padding: 15px 25px;
    }

    .my_card{ 
        border-radius: 15px;
        background-color: white;

        h3{ 
            font-weight: 600;
        }
    }
</style>

