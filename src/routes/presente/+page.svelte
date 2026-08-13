<script lang="ts">
  import Correct from "$lib/correct.svg";
</script>

<section id="gifts">
  <div style="top: 28px; position: relative;">
    <h2
      class="display m"
      style="bottom: -8vw; position: relative; left: 5.5vw;"
    >
      IDEIAS DE
    </h2>
    <h2 class="great">Presentes</h2>
  </div>

  <div id="presentes">
    <div class="left">
      <img src={Correct} alt="Correct" />
      <p class="display p">ACESSÓRIOS PRATA</p>
    </div>
    <div class="right">
      <img src={Correct} alt="Correct" />
      <p class="display p">CALÇADO Nº 36</p>
    </div>
    <div class="left">
      <img src={Correct} alt="Correct" />
      <p class="display p">ROUPAS PP/P</p>
    </div>
    <div class="right">
      <img src={Correct} alt="Correct" />
      <p class="display p">PERFUME</p>
    </div>
    <div class="left">
      <img src={Correct} alt="Correct" />
      <p class="display p">ITENS CATÓLICOS</p>
    </div>
    <div class="right">
      <img src={Correct} alt="Correct" />
      <p class="display p">BODY SPLASH</p>
    </div>
  </div>

  <a href="./"><button class="display m">voltar</button></a>
</section>

<style lang="css">
  @import url("https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=Great+Vibes&display=swap");

  a button{
    background-color: #e8c44b;
    color: #001d3d;
    border: none;
    padding: 1vw 2vw;
    border-radius: 5px;
    cursor: pointer;

    transition: all 0.3s ease-in-out;
  }

  #gifts {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 48px;

    padding: 5vw;
  }

  .left {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
  }

  .right {
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
    justify-content: space-around;
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

  h2 {
    font-size: 20vw;
    margin: 0;
  }

  /*ESTILOS*/

  #presentes {
    display: flex;
    flex-direction: column;
    gap: 48px;

    div {
      display: flex;
      align-items: center;
      justify-content: space-around;
      gap: 32px;
    }
  }

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
</style>
