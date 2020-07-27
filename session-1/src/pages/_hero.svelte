<script>
  import Input from './_components/input.svelte'
</script>

<style>
  .hero {
    background-color: #EFEFEF;
    padding-top: 11.5px;
    padding-bottom: 45px;
  }

  h1 {
    color: #2a2a2a;
    font-size: 47px;
    margin-top: -26px;
    margin-bottom: 26px;
    letter-spacing: -1.2px;
  }

  p {
    color: #888888;
    font-size: 20px;
    margin-top: 0px;
    margin-bottom: 0px;
    letter-spacing: -0.8px;
    line-height: 25px;
  }

  .input-container {
    margin-top: 60px;
  }


  @media(min-width: 992px) {
    .container {
      display: grid;
      grid-template-columns: repeat(12, 1fr);
      grid-template-rows: 1fr;
      grid-column-gap: 30px;
      align-items: center;
    }

    .hero-image {
      grid-column: 8/13;
    }

    .hero-content {
      grid-column: 1/7;
      grid-row: 1/2;
    }

    h1 {
      font-size: 60px;
      margin-top: 0px;
      margin-bottom: 18px;
    }

    p {
      font-size: 25px;
      letter-spacing: -1px;
      line-height: 30px;
    }
  }
</style>

<div class="hero">
  <div class="container">
    <div class="hero-image">
      <img src="/images/hero-img.png" alt="Hero Image">
    </div>

    <div class="hero-content">
      <h1 class="sofia-bold">Llevá tu talento al siguiente nivel</h1>
      <p class="sofia-light">Los tratamientos más eficaces al alcance de los profesionales de belleza y salud.</p>

      <div class="input-container">
        <Input placeholder="Ingresá el equipo que buscas"/>
      </div>
    </div>
  </div>
</div>
