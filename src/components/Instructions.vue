<template>
  <section class="instructions">
    <h1>Instructions</h1>
    <Instruction order="1" text="Adjust the oven rack to the lower-middle position and preheat oven to 350°F (177°C)." />
    <Instruction order="2" text="<b>Make the crust</b>: Using a food processor, pulse the graham crackers into crumbs. Pour into a medium bowl and stir in sugar and melted butter until combined. (You can also pulse it all together in the food processor.) Mixture will be sandy. Press firmly into the bottom and slightly up the sides of a 9-inch or 10-inch springform pan. No need to grease the pan first. I use the bottom of a measuring cup to pack the crust down tightly. Pre-bake for 8 minutes. Remove from the oven and place the hot pan on a large piece of aluminum foil. The foil will wrap around the pan for the water bath in step 4. Allow crust to slightly cool as you prepare the filling." />
    <Instruction order="3" text="<b>Make the filling</b>: Using a handheld or stand mixer fitted with a paddle attachment, beat the cream cheese and granulated sugar together on medium-high speed in a large bowl until the mixture is smooth and creamy, about 2 minutes. Add the sour cream, vanilla extract, and lemon juice then beat until fully combined. On medium speed, add the eggs one at a time, beating after each addition until just blended. After the final egg is incorporated into the batter, stop mixing. To help prevent the cheesecake from deflating and cracking as it cools, avoid over-mixing the batter as best you can." />
    <Instruction order="4" text="<b>Prepare the simple water bath (see note)</b> Boil a pot of water. You need 1 inch of water in your roasting pan for the water bath, so make sure you boil enough. I use an entire kettle of hot water. As the water is heating up, wrap the aluminum foil around the springform pan. Pour the cheesecake batter on top of the crust. Use a rubber spatula or spoon to smooth it into an even layer. Place the pan inside of a large roasting pan. Carefully pour the hot water inside of the pan and place in the oven. (Or you can place the roasting pan in the oven first, then pour the hot water in. Whichever is easier for you.)" />
    <Instruction order="5" text="Bake cheesecake for 55-70 minutes or until the center is almost set. When it’s done, the center of the cheesecake will slightly wobble if you gently shake the pan. Turn the oven off and open the oven door slightly. Let the cheesecake sit in the oven in the water bath as it cools down for 1 hour. Remove from the oven and water bath, then cool cheesecake completely at room temperature. Then refrigerate the cheesecake for at least 4 hours or overnight." />
    <Instruction order="6" text="Use a knife to loosen the chilled cheesecake from the rim of the springform pan, then remove the rim. Using a clean sharp knife, cut into slices for serving. For neat slices, wipe the knife clean and dip into warm water between each slice." />
    <Instruction order="7" text="Serve cheesecake with desired toppings. Cover and store leftover cheesecake in the refrigerator for up to 5 days." />

    <div class="link">
      <p class="link-source">Source: https://sallysbakingaddiction.com/classic-cheesecake/ </p>
    </div>
  </section>
</template>

<script>
import Instruction from './Instruction.vue';

export default {
  name: 'Instructions',
  components: {
    Instruction,
  }
}
</script>

<style scoped>
  .instructions {
    display: flex;
    flex-direction: column;
    text-align: initial;
    width: 100%;
  }
  
  .instructions h1 {
    font-family: 'Playfair Display';
    font-style: normal;
    font-weight: 700;
    font-size: 24px;
    line-height: 32px;
    color: var(--gray-900);
    padding: 28px 0;
  }

  .link .link-source {
    font-family: 'Montserrat';
    font-style: italic;
    font-weight: 400;
    font-size: 16px;
    line-height: 150%;
    color: var(--gray-600);
    margin-top: 26px;
    margin-bottom: 93px;
  }
</style>