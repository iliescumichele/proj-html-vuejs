<template>
  <nav class="container clearfix">
    <div class="nav-logo float-left">
        <h2><span>NEX</span><span>GEN</span></h2>
    </div>

    <div class="links float-right clearfix">
        <ul class="">
            <li><a href="#">HOME</a></li>
            <li><a href="#service">SERVICES</a></li>
            <li><a href="#">SKILLS</a></li>
            <li><a href="#partners">PARTNERS</a></li>
            <li><a href="#">BLOG</a></li>
        </ul>
        <p class="btn-get-in-touch">GET IN TOUCH</p>
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
        width: 50%;
        color: white;
    }

    .nav-logo{
        margin: 10px 0;
        opacity: 60%;

        h2{
            margin:  0;
            
            span{
                padding: 7.5px 0;
                padding-right: 5px;
            }
        }

        span:first-child{ 
            color: $colorCube_blueLagoon;
            background-color: $colorCube_blueLagoonAlpha;
            padding-left: 20px;
            border-radius: 44% 0 0 44%;
        }

        span:last-chlid{ 
            padding-left: 2px;
        }
    }

    .links{
        display: flex;
        justify-content: end;

        li{
            text-align: right;
            display: inline-block;
            margin: 15px 15px;
            list-style: none;

            a{
                color: white;
                text-decoration: none;
            }
            a:hover{
                cursor: pointer;
            }
        }
    }

    .btn-get-in-touch{
        margin-left: 5px;
        padding: 12px 20px;
        background-color: $colorCube_blueLagoon;
        border-radius: 3px;
    }

    .btn-get-in-touch:hover{ 
        transform: scale(1.02);
        cursor: pointer;
    }

</style>