<template>
  <header >
    <div class="container clearfix">
      <div class="header-sx float-left ">
        <span>Open Hours: {{mainInformationData.openDay}} - {{mainInformationData.closingDay}} - {{mainInformationData.openHour}} - {{mainInformationData.closingHour}}</span>
      </div>


      <div class="header-dx float-left ">
          <div class="icons-other-platforms">
            <a href=""><i class="fa-brands fa-facebook-f"></i></a>
            <a href=""><i class="fa-brands fa-twitter"></i></a>
            <a href=""><i class="fa-brands fa-linkedin-in"></i></a>
          </div>

          <div class="contact-email">
          <i class="fa-solid fa-envelope"></i>
            <span>{{mainInformationData.email}}</span>
          </div>

          <div class="contact-number">
            <i class="fa-solid fa-phone"></i>
            <span>{{mainInformationData.phone}}</span>
          </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'headerComponent',
  data(){
    return{
      mainInformationData: {
        "phone": "+1 (305) 1234-5678",
        "email": "hello@example.com",
        "openHour": "9.00",
        "closingHour": "18:00",
        "openDay": "Mon",
        "closingDay": "Sat"
      }
    }
  }
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/vars.scss';


  header{
    height: 65px;
    color: $colorCube_saltpan;
    background-color: #1c303c;

    .container{
      height: 100%;
    }
  }

  .header-sx, .header-dx{
    width: 50%;
    height: 100%;
    display: flex;
    align-items: center;
  }

  .header-dx{
    flex-direction: row-reverse;

    .contact-number, .contact-email, .icons-other-platforms{
      margin-left: 25px;

      i{
        margin: 0 10px;
      }
    }

    .icons-other-platforms{
      a{ 
        color: $colorCube_saltpan;
        padding: 0 12px;
      }

      i:hover{ 
        transform: scale(1.2);
      }
    }
  }
</style>