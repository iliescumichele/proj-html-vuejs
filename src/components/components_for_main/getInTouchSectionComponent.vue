<template>
  <section id="get-in-touch">
        <div class="container d-flex align-items-center justify-content-center h-100">
            <div class="row h-75">
                <div class="col-8 h-100 ">
                    <div class="top-title-sx">
                        <h4>SEND A MESSAGE</h4>
                        <h2 class="my-3">Get in <span>Touch</span></h2>
                        <p class="">We will respond to your message as soon as possible.</p>
                    </div>
                    <form class="form">
                        <div class="container fluid">
                            <div class="row">
                                <div class="col-6">
                                    <input type="text" class="form-control w-100" id="inmputName" placeholder="Name">
                                </div>
                                <div class="col-6">
                                    <input type="email" class="form-control w-100" id="inputEmail" aria-describedby="Email" placeholder="Email">
                                </div>
                                <div class="col-6">
                                    <input type="text" class="form-control w-100" id="inmputPhone" placeholder="Phone">
                                </div>
                                <div class="col-6">
                                    <select class="form-select w-100" aria-label="Default select example">
                                        <option disabled selected>More info</option>
                                        <option value="1">One</option>
                                        <option value="2">Two</option>
                                        <option value="3">Three</option>
                                    </select>
                                </div>
                                <div class="col-12">
                                    <input type="text" class="form-control w-100" id="inmputPhone" placeholder="Message">
                                </div>
                            </div>
                            <button type="submit" class="btn mt-4">SEND</button>
                        </div>
                    </form>
                </div>
                <div class="col-4">
                    <p class="top-title-dx">Example Inc.</p>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                    <div class="incons-and-contacts">
                        <div class="phone mt-4">
                            <i class="fa-solid fa-phone"></i>
                            <span>+1 (305) 1234-5678</span>
                        </div>
                        <div class="mail my-4">
                            <i class="fa-solid fa-envelope"></i>
                            <span>hello@example.com</span>
                        </div>
                        <div class="address mb-3">
                            <i class="fa-solid fa-location-dot"></i>
                            <span>Main Avenue, 987</span>
                        </div>
                    </div>
                    <a href="#" class="btn my-4">VIEW MAP</a> 
                </div>
            </div>
        </div>
  </section>
</template>

<script>
export default {
    name: 'getInTouchSectionComponent'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/vars.scss';

    section{ 
        height: 700px;
        background-color: $colorCube_saltpan;
    }

    .top-title-sx{ 
        margin-left: 24px;
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
    }

    form{
        .col-6{
            margin: 8px auto;
        }

        .col-12{
            margin-top: 8px;
        }

        input, select{ 
            opacity: .95;
            height: 50px;
            background-color: #dce2db;
            border: none;
        }

        .col-12 input{
            height: 163px;
        }
        .btn{ 
            background-color: $colorCube_blueLagoon;
            color: $medinCut_grayNurse;
            padding: 12px 20px;
        }
    }  

    .col-4{
        padding-left: 20px;

        p.top-title-dx{ 
            font-size: 1.3rem;
            font-weight: bold;
            color: black;
        }

        p{
            font-size: 1.15rem;
            color: $colorCube_manatee;
        }

        .incons-and-contacts{ 
            color: $materialDesign_elfGreen;
            font-size: 1.35rem;

            i{ 
                background-color: $materialDesign_elfGreenAlpha;
                padding: 15px;
                border-radius: 50%;
                margin-right: 12px;
            }
        }

        .btn{ 
            color: $materialDesign_elfGreen;
            border: 1px solid $materialDesign_elfGreen;
            padding: 12px 25px;
        }
    }

</style>