<template>
  <nav class="container">
    <div class="row row-cols-2">
        <div class="col nav-logo">
            <h3><span>NEX</span><span>GEN</span></h3>
        </div>

        <div class="col links">
            <ul class="nav d-flex align-items-center ">
                <li class="nav-item">
                    <a class="nav-link" href="#">HOME</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#services">SERVICES</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#skills">SKILLS</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#partners">PARTNERS</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link ">BLOG</a>
                </li>
            </ul>
            <button type="button" class="btn" href="#get-in-touch">GET IN TOUCH</button> 
        </div>
    </div>


  </nav>
</template>

<script>
export default {
    name: 'navComponent'
}
</script>

<style lang="scss" scoped>
  @import '../../assets/style/vars.scss';

    .links, .nav-logo{
        color: $medinCut_grayNurse;
    }

    .nav-logo{
        display: flex;
        align-items: center;
        margin: 10px 0;
        opacity: 60%;

        h2{
            font-weight: bolder;
            color: $medinCut_grayNurse;

            span{
                padding: 7.5px 0;
                padding-right: 5px;
            }
        }

        span:first-child{ 
            color: $materialDesign_morningGlory;
            background-color: $colorCube_blueLagoonAlpha;
            padding: 6px 5px 6px 20px;
            border-radius: 30px 0 0 30px;
        }

        span:last-chlid{ 
            padding-left: 2px;
        }
    }



    .links{ 
        height: 100%;
        display: flex;
        justify-content: end;
        align-items: center;

        a{
            font-weight: bold;
            color: $medinCut_grayNurse;
            text-decoration: none;
        }
        a:hover{
            cursor: pointer;
        }
    }

    .btn{
        color: $medinCut_grayNurse;
        padding: 10px 18px;
        font-weight: bold;
        background-color: $colorCube_blueLagoon;
    }

    .btn-general:hover{
        transform: scale(1.02);
        cursor: pointer;
    }

</style>