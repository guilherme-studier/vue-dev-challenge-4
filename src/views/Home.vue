<template>
  <Header />
  <Ingredients />
  <Instructions />
  <footer>
    <p>created by <b>Guilherme</b> - devChallenges.io</p>
  </footer>
</template>

<script>
import Header from '../components/Header.vue';
import Ingredients from '../components/Ingredients.vue';
import Instructions from '../components/Instructions.vue';

export default {
  name: 'Home',
  components: {
    Header,
    Ingredients,
    Instructions,
  }
}
</script>

<style scoped>
  footer p {
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 17px;
    /* identical to box height */

    text-align: center;
    color: var(--gray-700);
  }
</style>