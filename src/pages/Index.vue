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
        <div class="contact">
          <address>5036 Main St, Machester Center, VT 05255</address>
          <a href="tel:802-768-8141">802 768 8141</a>
        </div>
        
        <div class="hours">
          <p>Wednesday - Saturday</p>
          <time datetime="11:30">11:30 AM</time> - <time datetime="20:00">8:00 PM</time>
          <p>Sunday</p>
          <time datetime="11:30">11:30 AM</time> - <time datetime="15:00">3:00 PM</time>
          <p>Monday, Tuesday</p>
          <time>Closed</time>
        </div>

        <Menu/>
      </aside>
    </section>

    <footer class="full">
      <p>
        Cilantro is more than a delicious herb. It is more than a fast, casual restaurant in Manchester VT. It is so much more than the hard work and commitment we put into the restaurant every day. To us, and hopefully to all our loyal customers, Cilantro is a step. It is a step towards a promise that we will continue to be sustainable, local and committed to improving the prosperity of our wonderful town. We are local. Locally focused in the ingredients we use, locally focused in the charities we support, and locally focused in the people we serve. Together we promise to support the town and area that we are so humbly supported by. We also promise to do so in a manner that is kind to this sweet, sweet earth. With your help and our commitment, together we will all prosper.
      </p>

      <Menu/>
      <LogoIcon/>
    </footer>
  </Layout>
</template>

<script>
import LogoIcon from "~/components/LogoIcon";
import CilantroIcon from "~/components/CilantroIcon";
import Menu from "~/components/Menu";

export default {
  components: {
    LogoIcon, 
    CilantroIcon,
    Menu
  },
  metaInfo: {
    title: 'Home'
  }
}
</script>

<style lang="scss" scoped>
.hero {
  
  h1 {
    font-size: 70px;
    margin: 15px;

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
      }
    }
  }

  aside {
    background: black;
    padding: 10px;
    position: absolute;
    text-align: center;
    bottom: 5%;
    width: 250px;

    @media screen and (min-width: 400px) {
      bottom: 10%;
      width: 200px;
    }

    .contact {
      padding: 10px 0;

      a {
        color: white;
      }
    }


    .hours {
      p {
        margin: 0;
      }

      time + p {
        margin-top: 5px;
      }
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
    
    @media screen and (max-width: 800px){
      line-height: 150%;
    }

    @media screen and (min-width: 800px) {
      padding-top: 50px;
      padding-bottom: 50px;
    }

    + a {    
      padding-bottom: 100px;
    }
  }

  svg {
    position: absolute;
    width: 150px;
    bottom: 50px;

    @media screen and (min-width: 800px) {
      width: 150px;
      padding-bottom: 50px;
    }
  }
}
</style>
