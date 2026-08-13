<script lang="ts">
  import Icon from "$lib/icon.svg";
  import Presente from "$lib/presente.svg";
</script>

<div id="intro">
  <p class="display pp">CONFIRMAR PRESENÇA ATÉ 10/09</p>
  <p class="display">
    VOCÊ ESTÁ CONVIDADO PARA CELEBRAR UM MOMENTO MUITO ESPECIAL!
  </p>
</div>

<div id="titulo">
  <h2 class="great">15 anos</h2>
  <h1 id="tt2" class="display">DA RAFAELA</h1>
</div>

<p>
  SERÁ UMA NOITE INESQUECÍVEL, MARCADA POR SONHOS, ELEGÂNCIA E MUITA EMOÇÃO!
</p>

<p class="display pp">CLIQUE EM TUDO QUE PISCA PARA INTERAGIR!</p>

<div id="data">
  <p class="great m">sábado</p>
  <a
    class="display m pulso"
    target="_blank"
    href="https://calendar.google.com/calendar/event?action=TEMPLATE&amp;tmeid=Nm9mY2x2ZWNvcnE1NTVuMTk5bWRqbjRyMGogbWUyNTAzMjAwOEBt&amp;tmsrc=me25032008%40gmail.com"
    >26 DE SETEMBRO DE 2026</a
  >
  <p class="great m">às 19:30</p>
</div>

<div id="local">
  <p class="display p">QUITAÚNA - OSASCO</p>
  <a target="_blank" href="https://maps.app.goo.gl/N9XWgAoXrPCYjUV37"
    ><h3 class="display g pulso">BUFFET URIEL</h3></a
  >
  <p class="display pp">Rua General Florêncio, 868</p>
</div>

<section id="manual">
  <div>
    <p class="display m">MANUAL DO CONVIDADO</p>
    <hr />
  </div>

  <div id="traje">
    <p class="display p" style="margin-left: 10vw; margin-bottom: -1.5vh;">
      TRAJE SUGERIDO
    </p>
    <p class="great gg" style="margin-left:-10vw">Esporte fino</p>
  </div>

  <p>SUA PRESENÇA É MUITO IMPORTANTE PARA MIM!</p>

  <a
    target="_blank"
    href="https://wa.me/5511974135767?text=Olá%20Gostaria%20de%20confirmar%20minha%20presença%20no%20seu%20aniversário!"
  >
    <div id="presença">
      <div class="img"><img src={Icon} alt="Ícone" /></div>

      <div>
        <p class="display p" style="margin-left: 12vw; margin-bottom: -5vw;">
          CONFIRME SUA
        </p>
        <p class="great gg" style="margin-left: -15vw;">Presença</p>
      </div>
    </div></a
  >

  <p>CASO TENHA DUVIDAS, VEJA IDEIAS DE PRESENTES</p>

  <a href="/presente">
    <div id="presente">
      <div class="img"><img src={Presente} alt="Ícone" /></div>
      <div>
        <p class="display p" style="margin-left: 10vw; margin-bottom: -5vw;">
          IDEIAS DE
        </p>
        <p class="great gg" style="margin-left: -10vw;">Presentes</p>
      </div>
    </div></a
  >
</section>

<div id="assinatura">
  <p class="display p" style="margin-left: 12vw; margin-bottom: -3vw;">
    COM AMOR,
  </p>
  <p class="great gg" style="margin-left: -12vw;">Rafinha</p>
</div>

<style lang="css">
  @import url("https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=Great+Vibes&display=swap");

  /*CLASSES*/

  #presença {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
  }

  #presente {
    display: flex;
    justify-content: space-around;
    flex-direction: row-reverse;
  }

  .img {
    background-color: #ffc300;
    width: 10vw;
    height: fit-content;
    border-radius: 100%;
    padding: 3vw;
    display: flex;

    box-shadow: #001d3d 0 0 50px;

    animation: pulse-shadow 2s ease-in-out infinite;

    img {
      width: 100%;
      height: 100%;
    }
  }

  .pulso {
    animation: pulse-shadow-text 3s ease-in-out infinite;
  }

  @keyframes pulse-shadow {
    0%,
    100% {
      box-shadow: #001d3d 0 0 30px;
    }

    50% {
      box-shadow:
        #001d3d 0 0 50px,
        #ffc300 0 0 20px;
    }
  }

  @keyframes pulse-shadow-text {
    0%,
    100% {
      text-shadow: #001d3d 0 0 30px;
    }

    50% {
      text-shadow:
        #001d3d 0 0 50px,
        #ffc300 0 0 20px;
    }
  }

  #manual {
    display: flex;
    flex-direction: column;
    gap: 80px;
  }

  #intro {
    display: flex;
    flex-direction: column;
    gap: 8px;
  }

  /*INDIVIDUAIS*/

  p,
  h1,
  h2 {
    color: #ffc300;
  }

  a {
    color: #ffd60a;
    text-decoration: none;
  }

  h2 {
    font-size: 20vw;
    text-align: left;
  }

  hr {
    color: #ffc300;
    border: 0.5px solid #ffc300;
    margin: 2px;
  }

  /*TAMANHOS DE FONTES*/
  .pp {
    font-size: 3vw;
  }

  .p {
    font-size: 5vw;
  }

  .m {
    font-size: 6vw;
  }

  .g {
    font-size: 9vw;
  }

  .gg {
    font-size: 12vw;
  }

  /*ESTILOS*/

  .display {
    font-family: "DM Serif Display", serif;
    font-weight: 400;
    font-style: normal;
    margin: 0;
  }

  .great {
    font-family: "Great Vibes", cursive;
    font-weight: 400;
    font-style: normal;
    margin: 0;
  }

  #tt2 {
    font-size: 12vw;
    margin-top: -5vh;
    text-align: left;
  }
</style>
