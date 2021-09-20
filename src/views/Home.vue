<template>
  <div class="home">
    <img src="@/assets/images/casal.jpg">
    <h1 class="name-casal">Chá Cofrinho</h1>
    <p>
      Estamos a um passo do SIM, <br>
      mas antes queremos sua presença no nosso chá.<br>
      12/12/2021 às 14:00 horas.
    </p>

    <h2></h2>

    <div class="wrapper-counter">
      <CountdownTeste deadline="December 12, 2021"></CountdownTeste>
    </div>

    <p>
      Sua presença é nosso maior presente,<br>
      Mas se tiver um troquinho sobrando,
      haverá um cofre para que você deposite a quantia que quiser.
    </p>

    <h1 class="lua-mel">Ajude os noivos com a lua de mel!</h1>

    <div class="instagram">
      <p>Compartilhe este dia com muitas fotos e marque o nosso Instagram</p>

      <a href="https://www.instagram.com/xuxu_0116/" target="_blank">
        <img src="@/assets/images/instagram.svg">
        @xuxu_0116
      </a>
    </div>

    

    <div class="wrapper-map">
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3657.258983935291!2d-46.90684874902939!3d-23.559140284608837!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94cf06d36df58e51%3A0xfebf70863e5186b1!2sR.%20Jarama%2C%2068%20-%20Jardim%20Sao%20Joao%2C%20Jandira%20-%20SP%2C%2006634-020!5e0!3m2!1spt-BR!2sbr!4v1631674047237!5m2!1spt-BR!2sbr" width="100%" height="350" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
    </div>
  </div>
</template>

<script>
import CountdownTeste from '@/components/CountdownTeste.vue'

export default {
  name: 'Home',

  components: { CountdownTeste },
}
</script>

<style lang="scss" scoped>
.home {
  max-width: 1200px;
  padding: 20px;
  margin: 0 auto;

  h1 {
    margin-top: 20px;
    margin-bottom: 10px !important;
    font-family: 'Amatic SC', cursive;

    &.name-casal {
      font-size: 45px;
      text-align: center;
    }

    &.lua-mel {
      font-size: 28px;
      margin-bottom: 20px !important;
    }
  }

  p {
    text-align: center;
    font-size: 24px;
    font-family: 'Cormorant Garamond', serif;
  }

  img {
    max-width: 1200px;
    width: 100%;

    &.porquinho {
      max-width: 300px;
    }
  }

  .wrapper-counter {
    background: url('../assets/images/folhas/plaquinha.png') top center no-repeat;
    padding-top: 106px;
    padding-left: 15px;
    min-height: 160px;
    width: 100%;
    max-width: 360px;
    margin: 0 auto 30px;

    @media(max-width: 768px) {
      margin-left: -15px;
    }

  }

  .instagram {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 30px;

    p {
      margin: 0;
    }

    a {
      font-family: 'Cormorant Garamond', serif;
      font-size: 22px;
      color: #000;
      margin-left: 5px;
      display: flex;
      justify-content: center;
      align-items: center;

      img {
        max-width: 20px;
        margin-right: 5px;
        margin-bottom: -5px;
      }

    }

    @media(max-width: 768px) {
      flex-direction: column;
    }
  }
}
</style>
