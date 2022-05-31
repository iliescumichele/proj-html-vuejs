<template>
    <section id="newsletter">
        <div class="container d-flex align-items-center justify-content-center h-100">
            <div class="row row-cols-2">
                <div class="col info">
                    <h4>NEWSLETTER</h4>
                    <h2 class="my-3"><span>Know</span> first</h2>
                    <p class="">Follow closely and receive content about our company and the nes of the current market.</p>
                </div>
                <div class="col form">
                    <form>
                        <div class="mb-3">
                          <input type="text" class="form-control" id="inmputName" placeholder="Name">
                        </div>
                        <div class="mb-3">
                          <input type="email" class="form-control" id="inputEmail" aria-describedby="Email" placeholder="Email">
                        </div>
                        <button type="submit" class="btn">SUBSCRIBE</button>
                    </form>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    nmae: 'newsletterComponent'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/vars';

    section{ 
        height: 450px;
        background-image: url('../../assets/img/bg-1.jpg');
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
    }

    .info{ 
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
                background-color: $materialDesign_elfGreenAlpha;
            }
        }

        p{
            font-size: 1.15rem;
            color: $colorCube_manatee;
        }

    }
    
    form{
        input{ 
            opacity: .5;
            height: 60px;
        }
        .btn{ 
            background-color: $colorCube_blueLagoon;
            color: $medinCut_grayNurse;
            padding: 12px 20px;
        }
    }  
</style>