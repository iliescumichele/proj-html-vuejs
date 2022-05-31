<template>
  <section id="latest-news">
    <meta name="metro4:init" content="false">
    <div class="container">
        <div class="text-news">
            <h4>OUR EDITORIAL CONTENT</h4>
            <h2 class="my-4">Latest <span>News</span></h2>
            <div class="litle-text-and-button-underlatest-news-title mt-4">
                <p class="">Every week we publish content about what is best in the business world.</p>
                <button type="button" class="btn">SEE ALL</button> 
            </div>

            <div class="cards container-fluid ">
                <div class="row row-cols-3">
                    <div class="col position-relative">
                        <div class="card-background">
                            <img class="" src="../../assets/img/news-1.jpg" alt="">
                            <div class="card-img-dim position-absolute">
                                <div class="card-text">
                                    ciao
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'latestNewsSectionComponent'
};
</script>

<style lang="scss" scoped>
@import '../../assets/style/vars';

    section{
        height: 700px;
        background-color: #ffffff;
    }

    .text-news{
        padding-top: 100px;

        h4{ 
            font-size: 0.9rem;
            font-weight: 800;
            color: $materialDesign_elfGreen;
        }
        
        h2{
            font-size: 3rem;
            font-weight: 800;

            span{ 
                color: $materialDesign_elfGreen;
                background-color: $materialDesign_elfGreenAlpha;
            }
        }

        p{
            font-size: 1.15rem;
            color: $colorCube_manatee;
        }

        .litle-text-and-button-underlatest-news-title{ 
            display: flex;
            justify-content: space-between;
            align-items: center;

            .btn{ 
                background-color: $colorCube_blueLagoon;
                color: $medinCut_grayNurse;
                padding: 9px 20px;
            }
        }
    }

    .cards{ 
        .card-background{ 
            height: 300px;
            border-radius: 15px;
            
            img{ 
                width: 100%;
                background-repeat: no-repeat;
                background-position: center;
                background-size: cover;
                overflow: hidden;
                filter: brightness(0.6);
            }

            .card-img-dim{ 
                background-color: rgba(0, 0, 0, 0.6);
            }
        }
    }
</style>