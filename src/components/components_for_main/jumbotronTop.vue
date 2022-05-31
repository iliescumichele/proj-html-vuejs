<template>
    <div class="jumbotron">

        <div class="jumbo-content">

                <navComponent id="nav"/>

                <div class="bigText container d-flex align-items-center justify-content-center h-75">
                    <div class="row">
                        <div class="col">
                            <!-- colonna sx vuota -->
                        </div>
                        <div class="col-5 position-relative">
                            <div class="background-for-logistic"></div>
                            <h2><span></span>Logistics that goes further.</h2>
                            <p class="py-4">For 20 years working with the most innovative inthe field of transport.</p>
                            <div class="buttons">
                                <button type="button" class="btn">GET IN TOUCH</button>
                                <button type="button" class="btn">READ MORE</button>
                            </div>
                        </div>
                    </div>
                </div>

        </div>

    </div>
</template>

<script>
import navComponent from './navComponent.vue'


export default {
    name: 'jumbotronTop',
    components: {
    navComponent
  }
}

</script>

<style lang="scss" scoped>
@import '../../assets/style/vars.scss';

    .jumbotron{
        height: 800px;
        background-image: url(../../assets/img/jumbo.jpg);
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;

        .jumbo-content{
            height: 100%;
            background-color: rgba(0, 0, 0, 0.6);
        }
    }

    #nav{ 
        padding: 20px 0;
    }

    .bigText{
        .col-5{ 
        }

        .background-for-logistic{
            background-color: $colorCube_blueLagoonAlpha;
            height: 35px;
            width: 320px;
            position: absolute;
            top: 40px;
            left: 16px;
        }

        h2{ 
            font-size: 4rem;
            font-weight: 800;
            color: white;
        }

        p{ 
            font-size: 1.3rem;
            font-weight: 100;
            color: $medinCut_grayNurse;
            opacity: .8;
        }
    }   

    .buttons{
        .btn{ 
            color: $medinCut_grayNurse;
        }

        .btn:first-child{
            background-color: $colorCube_blueLagoon;
        }

        .btn:last-child{
            margin-left: 25px;
            border: 2px solid $colorCube_blueLagoon;
        }
        
        a{
            font-weight: bold;
            text-decoration: none;
            color: $colorCube_saltpan;
        }

        .btn:hover{
            transform: scale(1.02);
            cursor: pointer;
        }
    }

</style>