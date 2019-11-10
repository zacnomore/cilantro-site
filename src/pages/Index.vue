<template>
  <Layout>
    <section class="full hero">
      <g-image alt="An illustration of a sugar skull, a painted skull in celebration of Día de los Muertos" src="~/assets/SugarSkull.jpg" />
      <header>
        <h1>Mexican Street Food</h1>
        <p>Local. Sustainable. Authentic.</p>
      </header>
    </section>
    <header class="band">Step One</header>
    <section class="grid thirds">
      <div class="tile">
        <g-image alt="" src="~/assets/Burrito.jpg" />
        <div class="text">
          <h2>Burrito</h2>
          <p>Flour tortilla rolled up with rice, beans, meat, salsa, cheese, lettuce, sour cream and house sauce</p>
        </div>
      </div>
      <div class="tile">
        <g-image alt="" src="~/assets/HillOfBeans.jpg" />
        <div  class="text">
          <h2>Hills of Beans</h2>
          <p>Deconstructed burrito (no tortilla)</p>
        </div>
      </div>
      <div class="tile">
        <g-image alt="" src="~/assets/Salad.jpg" />
        <div  class="text">
          <h2>Salad</h2>
          <p>Chopped romaine, meat, cheese, roasted corn, black beans, pickled onions, cilantro-avocado dressing, sour cream, tosted pepitas</p>
        </div>
      </div>
      <div class="tile">
        <g-image alt="" src="~/assets/Americano.jpg" />
        <div  class="text">
          <h2>Taco Americano</h2>
          <p>Flour tortilla stuffed with meat, salsa, cheese, lettuce, sour cream and house sauce</p>
        </div>
      </div>
      <div class="tile">
        <g-image alt="" src="~/assets/StreetTacos.jpg" />
        <div  class="text">
          <h2>Street Taco</h2>
          <p>Corn tortilla stuffed with meat, salsa, fresh chopped cilantro and onions</p>
        </div>
      </div>
      <div class="tile">
        <g-image alt="" src="~/assets/MealDeal.jpg" />
        <div  class="text">
          <h2>Taco Meal Deal</h2>
          <p>Two tacos with a side of rice, beans and cheese</p>
        </div>
      </div>
    </section>

    <header class="band">Step Two</header>
    <section class="grid quarters">
      <div class="tile">
        <g-image alt="" src="~/assets/Meat.jpg" />
        <div class="text">
          <h2>Burrito</h2>
          <ul>
            <li>Chicken</li>
            <li>Pork</li>
            <li>Fresh chorizo</li>
            <li>Beef</li>
          </ul>
        </div>
      </div>
      <div class="tile">
        <g-image alt="" src="~/assets/Veggie.jpg" />
        <div  class="text">
          <h2>Veggie</h2>
          <ul>
            <li>Roasted mushroom</li>
            <li>Roasted corn</li>
            <li>Sliced avocado</li>
          </ul>
        </div>
      </div>
      <div class="tile">
        <g-image alt="" src="~/assets/Salsa.jpg" />
        <div  class="text">
          <h2>Salad</h2>
          <ul>
            <li>Fire roasted tomato (mild)</li>
            <li>Corn and black bean (medium)</li>
            <li>Tomatillo jalapeño (medium)</li>
            <li>Adobo sauce (medium)</li>
            <li>Tomato habañero (hot)</li>
          </ul>
        </div>
      </div>
      <div class="tile">
        <g-image alt="" src="~/assets/Cheese.jpg" />
        <div  class="text">
          <h2>Cheese</h2>
          <ul>
            <li>House queso fresco</li>
            <li>Monterey jack</li>
          </ul>
        </div>
      </div>
    </section>
    <footer class="full">
      <p>
        Cilantro is more than a delicious herb. It is more than a fast, casual restaurant in Manchester VT. It is so much more than the hard work and commitment we put into the restaurant every day. To us, and hopefully to all our loyal customers, Cilantro is a step. It is a step towards a promise that we will continue to be sustainable, local and committed to improving the prosperity of our wonderful town. We are local. Locally focused in the ingredients we use, locally focused in the charities we support, and locally focused in the people we serve. Together we promise to support the town and area that we are so humbly supported by. We also promise to do so in a manner that is kind to this sweet, sweet earth. With your help and our commitment, together we will all prosper.
      </p>
      <LogoIcon/>
    </footer>
  </Layout>
</template>

<script>
import { LogoIcon } from "~/components/LogoIcon";
import { CilantroIcon } from "~/components/CilantroIcon";
export default {
  components: [],
  metaInfo: {
    title: 'Cilantro'
  }
}
</script>

<style lang="scss" scoped>
.full {    
  height: 100vh;
  width: 100%;
  position: relative;

  header {
    position: absolute;
  }

  img {
    position: absolute;
    object-fit: cover;
    object-position: center;
    width: 100%;
    height: 100%;
    z-index: -2;
  }
}

img {
  filter: brightness(.35);
}

header.band {
  background: rgb(80, 181, 85);
}

.grid {
  display: flex;
  flex-wrap: wrap;
  align-content: stretch;
  min-height: 100vh;


  .tile {
    position: relative;
    flex-grow: 1;

    img {
      width: 100%;
      display: block;
      height: 100%;
      object-fit: cover;
      position: absolute;
      left: 0;
      right: 0;
      top: 0;
      bottom: 0;
      z-index: -1;
    }

    .text {
      margin: 20px;
    }

    h2 {
      margin: 0 0 40px 0;
      font-size: 80px;

      @media screen and (max-width: 800px) {
        margin: 0 0 30px 0;
        font-size: 60px;
      }
    }

    ul {
      list-style: none;
      margin: 0;
      padding: 0;
    }
  }

  &.thirds .tile{
    flex-basis: 33.33%;
    min-width: 350px;
  }


  &.quarters .tile{
    flex-basis: 25%;
    min-width: 250px;
  }

  &.thirds {
    flex-direction: column;
  }
}

footer {
  background: black;

  p {
    line-height: 200%;
  }
}
</style>