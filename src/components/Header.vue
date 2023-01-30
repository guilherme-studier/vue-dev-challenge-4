<template>
  <header>
    <div class="title">
      <h1>Classic Chessecake Recipe</h1>
    </div>
    <div class="subtitle">
      <img src="../assets/6dots.svg" alt="">
      <p>
        Look no further for a creamy and ultra smooth classic cheesecake recipe! Paired with a buttery graham cracker crust, no one can deny its simple decadence. For the best results, bake in a water bath.
      </p>
    </div>
    <div class="header__img">
      <img src="../assets/photo1.png" alt="">
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style scoped>
  header div {
    text-align: initial;
  }

  header .title h1 {
    font-family: 'Playfair Display';
    font-style: normal;
    font-weight: 700;
    font-size: 48px;
    line-height: 64px;
    margin-bottom: 12px;
  }


  header .subtitle {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    max-width: 592px;
    width: 100%;
  }

  header .subtitle p {
    font-family: 'Montserrat';
    font-style: italic;
    font-weight: 500;
    font-size: 14px;
    line-height: 17px;
    color: var(--gray-800);

    margin-block: 0;
  }

  header .subtitle img {
    margin-right: 12px;
    margin-top: 5px;
  }

  header .header__img {
    width: 100%;
    max-height: 470px;
    height: 100%;
    margin-top: 17px;
  }

  header .header__img img {
    margin-top: 26px;
    width: 100%;
  }

  @media (max-width: 800px) {
    header .title h1 {
      font-size: 24px;
      line-height: 32px;
      margin-bottom: 12px;
      margin-top: 32px;
    }

    header .subtitle {
      max-width: 320px;
      width: 100%;
    }

    header .subtitle p {
      font-weight: 500;
      font-size: 12px;
      line-height: 15px;
    }
  }
</style>