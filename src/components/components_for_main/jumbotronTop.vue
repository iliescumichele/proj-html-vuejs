<template>
    <div class="jumbotron">

        <div class="jumbo-content">

                <navComponent id="nav"/>

                <div class="bigText container d-flex align-items-center justify-content-center h-75">
                    <div class="row">
                        <div class="col-6">
                            <!-- colonna sx vuota -->
                        </div>
                        <div class="col-4">
                            <h2>Logistics that goes further.</h2>
                            <p>For 20 years working with the most innovative inthe field of transport.</p>
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
        height: 700px;
        background-image: url(../../assets/img/jumbo.jpg);
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;

        .jumbo-content{
            height: 700px;
            background-color: rgba(0, 0, 0, 0.6);
        }
    }

    #nav{ 
        padding: 20px 0;
    }

    .bigText{
        .empty-space{ 
            width: 50%;
        }

        h2{ 
            font-size: 4rem;
            font-weight: 800;
            color: white;
        }

        p{ 
            color: $medinCut_grayNurse;;
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