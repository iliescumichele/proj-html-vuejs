<template>
    <section id="skills">
        <div class="dots-top">
            <img src="../../assets/img/bullets.png" alt="">
        </div>
        

        <div class="text-info h-100 float-left">
            <div class="container h-100">
                <div class="row h-100">
                    <div class="col">
                        <!-- colonna a sx vuota -->
                    </div>
                    <div class="col-8 h-100 py-5">
                        <div class="text">
                            <h4>ABOUT THE NETWORK</h4>
                            <h2 class="my-3"><span>The</span> Company</h2>
                            <p class="my-3">With all this experties and capability comes an unrivalled commitment to customers services.</p>
                        </div>
                        <div class="container-fluid">
                            <div class="percentages my-5"> 

                            <cardPercentages 
                                v-for="(cardItem, index) in cardPercentagesList"
                                :key="`cardItem${index}`"
                                :cardData="cardItem"
                            />  
 
                            </div>
                        </div>

                    </div>
                </div>
            </div>
        </div>

        <div class="img-jumbo h-100 float-left">
            <!-- img a dx come background -->
        </div>

        <div class="dots-bottom">
            <img src="../../assets/img/bullets.png" alt="">
        </div>
    </section>
</template>

<script>
import cardPercentages from "./cards/cardPercentages.vue"

export default{
    name: 'theCompanySectionComponent',
    components: { cardPercentages },
    data(){
        return{
            cardPercentagesList: [
                {
                    "percentage": "90%",
                    "description": "Lorem ipsum dolor sit, amet consectetur adipisicing elit.",
                    "title": "Leadership"
                },
                {
                    "percentage": "80%",
                    "description": "Lorem ipsum dolor sit, amet consectetur adipisicing elit.",
                    "title": "Psichology"
                },
                {
                    "percentage": "50%",
                    "description": "Lorem ipsum dolor sit, amet consectetur adipisicing elit.",
                    "title": "Flexibility"
                },
            ]
        }
    }
}

</script>

<style lang="scss" scoped>
@import '../../assets/style/vars.scss';

    

    section{ 
        height: 800px;
        position: relative;

        .dots-top, .dots-bottom{
            position: absolute;
            opacity: 30%;
            left: 50%;
            transform: translate(-50%, -50%);

            img{
                width: 150px;
                height: 65px;
                object-fit: cover;
            }
        }

        .dots-top{
            top: -5px;
        }

        .dots-bottom{
            bottom: -60px;
        }

        .text-info{ 
            background-color: #070710;
            width: 50%;
        }

        .img-jumbo{
            width: 50%;
            background-image: url('../../assets/img/about-5.jpg');
            background-repeat: no-repeat;
            background-position: center;
            background-size: cover;
        }
    }

    .text-info{ 
        .col-8{ 

            h4{ 
                font-size: 0.9rem;
                font-weight: 800;
                color: $materialDesign_elfGreen;
            }
        
            h2{
                font-size: 3rem;
                font-weight: 800;
                color: white;

                span{ 
                    background-color: rgba(8, 129, 129, 0.35);
                }
            }

            p{ 
                font-size: 1.15rem;
                color: $colorCube_manatee;
            }
        }
    }



    
</style>