<template>
  <section class="content-ingredients">
    <div class="ingredients">
      <h1>Ingredients</h1>
      <h2>Graham Cracker Crust</h2>
      <Ingredient text="1 and 1/2 cups (150g) <b>graham cracker crumbs</b> (about 10 full sheet graham crackers)"/>
      <Ingredient text="5 Tablespoons (70g) <b>unsalted butter</b>, melted"/>
      <Ingredient text="1/4 cup (50g) <b>granulated sugar</b>"/>

      <h2>Cheesecake</h2>
      <Ingredient text="four 8-ounce blocks (904g) full-fat <b>cream cheese</b>, softened to room temperature"/>
      <Ingredient text="1 cup (200g) <b>granulated sugar</b>"/>
      <Ingredient text="1 cup (240g) full-fat <b>sour cream</b>, at room temperature"/>
      <Ingredient text="1 teaspoon <b>pure vanilla extract</b>"/>
      <Ingredient text="2 teaspoons <b>fresh lemon juice</b> (optional, but recommended)"/>
      <Ingredient text="3 large <b>eggs</b>, at room temperature"/>
      <Ingredient text="topping suggestions: <i>salted caramel, lemon curd, strawberry topping, chocolate ganache, red wine chocolate ganache, fresh fruit, whipped cream, or raspberry sauce</i> (recipe in notes) "/>
    </div>
    <Cooking />
    <div class="cooking">
      <Cook icon="restaurant_menu" title="Yields" subtitle="12 servings"/>
      <Cook icon="schedule" title="Prep Time" subtitle="45 minutes"/>
      <Cook icon="schedule" title="Cook time" subtitle="1 hour"/>
      <Cook icon="schedule" title="Total time" subtitle="7,75 hours"/>
    </div>
  </section>
</template>

<script>
import Ingredient from './Ingredient.vue';
import Cook from './Cook.vue';

export default {
  name: 'Ingredients',
  components: {
    Ingredient,
    Cook
  }
}
</script>

<style scoped>
  .content-ingredients {
    width: 100%;
    display: flex;
    margin-top: 48px;
  }

  section .ingredients {
    text-align: initial;
    max-width: 696px;
    width: 100%;
  }

  section .ingredients h1 {
    font-family: 'Playfair Display';
    font-style: normal;
    font-weight: 700;
    font-size: 24px;
    color: var(--gray-900);
  }

  section .ingredients h2 {
    font-family: 'Playfair Display';
    font-style: italic;
    font-weight: 400;
    font-size: 18px;
    margin-top: 32px;
    margin-bottom: 31px;
    color: var(--gray-900);
  }

  section .cooking {
    max-width: 216px;
    width: 100%;
  }

  section .cooking {
    width: 216px;
    height: 367px;

    background: #FFFFFF;
    box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.1);
    border-radius: 12px;

    display: flex;
    flex-direction: column;
    padding-left: 40px;
  }

  section .cooking div:first-child {
    margin-top: 57px;
  }

  section .cooking div {
    margin-top: 43px;
  }


  .icon-time {
    color: var(--gray-800);
  }

  .icon-restaurant {
    color: var(--orange-500)
  }

  @media (max-width: 700px) {
    section .ingredients h1 {
      font-weight: 700;
      font-size: 18px;
    }

    section .ingredients h2 {
      font-weight: 400;
      font-size: 16px;
      margin-top: 13px;
      margin-bottom: 24px;
    }


    .content-ingredients {
      flex-flow: column-reverse;
    }

    .content-ingredients .cooking {
      max-width: 360px;
      width: 100%;
      height: fit-content;
      box-shadow: none;
      flex-direction: row;
      padding: 0;
      margin: 0;
      flex-wrap: wrap;
      justify-content: space-between;
    }

    .content-ingredients .cooking div:first-child {
      margin-top: 0;
      margin-bottom: 20.75px;
      max-width: 333.71px;
      width: 100%;
      justify-content: initial;
    }

    .content-ingredients .cooking div {
      margin: 0;
      padding: 0;
      margin-bottom: 30.25px;
      justify-content: space-between;
    }
  }
</style>