<template>
  <header >
    <div class="container clearfix ">
      <div class="header-sx float-left ">
        <p>Open Hours: Mon - Sat - 9.00 - 18:00</p>
      </div>


      <div class="header-dx float-left ">
          <div class="icons-other-platforms">

          </div>

          <div class="contact-email">
            <span>hello@example.com</span>
          </div>

          <div class="contact-number">
            <span>+1 (305) 1234-5678</span>
          </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'headerComponent'
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/vars.scss';


  header{
    height: 75px;
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
    }
  }
</style>