<template>
  <div class="instruction">
      <h2 class="order">{{ order }}</h2>
      <p v-html="text"></p>
    </div>
</template>

<script>
export default {
  name: 'Instruction',
  props: {
    order: {
      type: Number,
      default: null
    },
    text: {
      text: {
        type: String,
        default: null
      }
    }
  }
}
</script>

<style scoped>
  .instruction {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
  }

  .instruction .order {
    font-family: 'Playfair Display';
    font-style: normal;
    font-weight: 700;
    font-size: 24px;
    background: var(--orange-500);
    border-radius: 6px;
    padding: 0px 13px 6px 13px;;
    color: var(--white);
    margin-right: 15px;
  }

  .instruction p {
    width: 528px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 20px;
    margin-bottom: 31px;
  }

  @media (max-width: 700px) {

    .instruction p {
      width: 300px;
      margin-bottom: 11px;
    }
  }
</style>