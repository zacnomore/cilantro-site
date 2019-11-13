<template>
  <Layout>
    <section class="full hero">
      <g-image alt="An illustration of a sugar skull, a painted skull in celebration of Día de los Muertos" src="~/assets/SugarSkull.jpg" />
      <header>
        <h1>
          Mexican Street Food
        </h1>
        <p>Local. Sustainable. Authentic.</p>
      </header>
      <aside>
        <LogoIcon/>
        <address>5036 Main St, Machester Center, VT 05255</address>
        
        <div class="hours">
          <p>Every Day</p>
          <time datetime="11:30">11:30 AM</time> - <time datetime="20:00">8:00 PM</time>
        </div>
      </aside>
    </section>

    <header class="band">
      <CilantroIcon/>
      Step One
    </header>
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

    <header class="band">
      <CilantroIcon/>
      Step Two
    </header>
    <section class="grid quarters">
      <div class="grid halves">
        <div class="tile">
          <g-image alt="" src="~/assets/Meat.jpg" />
          <div class="text">
            <h2>Meat</h2>
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
      </div>
      <div class="grid halves">
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
      </div>
    </section>


    <header class="band">
      <CilantroIcon/>
      Step Three
    </header>
    <section class="grid thirds vertical">
      <div class="tile">
        <g-image alt="" src="~/assets/Extras.jpg" />
        <div class="text">
          <h2>Extras</h2>
          <ul class="two-col">
            <li>Pickled Onions</li>
            <li>Sliced Jalapeño</li>
            <li>Roasted Corn</li>
            <li>Roasted Mushrooms</li>
            <li>Extra Cheese</li>
            <li>Sliced Avocado</li>
            <li>Extra Meat</li>
          </ul>
        </div>
      </div>
      <div class="tile">
        <g-image alt="" src="~/assets/Salsa.jpg" />
        <div  class="text">
          <h2>Corn Chips and Salsa</h2>
          <p>Corn chips with your choice of house made salsa</p>
        </div>
      </div>
      <div class="tile">
        <g-image alt="" src="~/assets/Beverages.jpg" />
        <div  class="text">
          <h2>Beverages</h2>
          <ul class="two-col">
            <li>Fresh brewed iced tea</li>
            <li>House made limeade</li>
            <li>Select beer</li>
            <li>Wine</li>
            <li>Soda</li>
            <li>Water</li>
            <li>Seltzer</li>
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
import LogoIcon from "~/components/LogoIcon";
import CilantroIcon from "~/components/CilantroIcon";

export default {
  components: {
    LogoIcon, 
    CilantroIcon
  },
  metaInfo: {
    title: 'Home'
  }
}
</script>

<style lang="scss" scoped>
.hero {
  
  h1 {
    font-size: 80px;
    margin: 30px;

    + p {
      line-height: 100%;
      font-size: 40px;
      margin: 0 30px;
    }
  }

  @media screen and (min-width: 1000px) {
    h1 {
      font-size: 120px;
      margin: 30px;

      + p {
        font-size: 60px;
        margin: 0 30px;
      }
    }
  }

  aside {
    background: black;
    padding: 10px;
    position: absolute;
    bottom: 10%;
    text-align: center;
    width: 200px;


    address {
      padding: 10px 0;
    }


    .hours p {
      margin: 0;
    }

    svg { 
      width: 100px;
    }

    @media screen and (min-width: 800px) {
      padding: 10px;

      svg { 
        width: auto;
      }
    }
  }
}


.full {    
  min-height: 100vh;
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
  color: black;
  display: flex;
  font-size: 20px;
  align-items: center;
  height: 30px;
  padding: 4px;

  > * {
    padding-right: 4px;
  }
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
      margin: 40px 20px;
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

      &.two-col{
        max-height: 8em;
        column-count: 2;
        max-width: 600px;
      }
    }
  }

  &.quarters > * {
    flex-basis: 50%;
    min-width: 250px;
    flex-direction: column;
    flex-grow: 1;

    @media screen and (min-width: 1000px) {
      flex-direction: row;
    }
  }

  &.thirds .tile{
    flex-basis: 0;
    min-width: 350px;
  }


  &.halves > * {
    flex-basis: 50%;
    min-width: 250px;
  }

  &.vertical {
    flex-direction: column;
  }
}

footer {
  background: black;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  position: relative;

  p {
    line-height: 250%;
    width: 80%;
    text-align: center;
    padding-bottom: 150px;
    padding-top: 50px;
    
    @media screen and (max-width: 800px){
      line-height: 150%;
    }
  }

  svg {
    position: absolute;
    width: 150px;
    bottom: 50px;
  }
}
</style>