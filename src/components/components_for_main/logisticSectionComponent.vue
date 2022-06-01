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
                
                <cardLogistics 
                    v-for="(cardItem, index) in cardLogisticsList"
                    :key="`cardItem${index}`"
                    :cardData="cardItem"
                />
                
            </div>
        </div>
    </section>
</template>

<script>
import cardLogistics from "./cards/cardLogistics.vue"

export default {
    name: 'logisticSectionComponent',
    components: { cardLogistics },
    data(){
        return{
            cardLogisticsList: [
                {
                    "thumb": "gallery-3.jpg",
                    "title": "Technology",
                    "description": "Focused on developing technology solutions adapted to our client's needs."
                },
                {
                    "thumb": "gallery-5.jpg",
                    "title": "Transport",
                    "description": "We develop operational strategies to improve logistical efficiency."
                }
            ]
        }
    }
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

    .my-card{ 
        border-radius: 15px;
        background-color: white;

        h3{ 
            font-weight: 600;
        }
    }
</style>

