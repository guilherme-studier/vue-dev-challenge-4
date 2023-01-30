<template>
  <div class="ingredients-checkbox">
    <div class="ingredients-input">
      <input type="checkbox" id="horns" name="horns">
    </div>
    <div class="ingredients-label">
      <label for="horns" v-html="text"></label>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Ingredients',
  props: {
    text: {
      type: String,
      default: null,
    }
  }
}
</script>

<style scoped>
  .ingredients-checkbox {
    display: flex;
    margin-bottom: 12px;
  }

  .ingredients-checkbox input {
    width: 21px;
    height: 21px;
  }

  .ingredients-checkbox .ingredients-input {
    align-items: flex-start;
  }

  .ingredients-checkbox .ingredients-label  {
    margin-left: 17px;
    margin-top: 5px;
    width: 554px;
  }

  .ingredients-checkbox .ingredients-label label {
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 25px;
    color: var(--gray-900);
  }

  @media (max-width: 700px) {
    .ingredients-checkbox .ingredients-label label {
      font-size: 14px;
    }

    .ingredients-checkbox .ingredients-label  {
      margin-left: 8px;
      margin-top: 3px;
    }
  }
</style>