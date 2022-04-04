<template>
<section class="snap">
<Header/>
</section>

<section class="snap">
<Slider />
</section>

<section class="snap">
<InfoWrapper />
</section>

<section class="snap">
<Offers  />
</section>

<section class="snap">
<OffersSecond />
</section>

<section class="snap">
<OffersThird />
</section>
<section class="snap">
<Contact />
</section>
</template>

<script>

import Header from "./components/Header.vue";
import Slider from "./components/Slider.vue";
import Offers from "./components/Offers.vue";
import OffersSecond from "./components/OffersSecond.vue";
import OffersThird from "./components/OffersThird.vue";
import InfoWrapper from "./components/InfoWrapper.vue";
import Contact from "./components/Contact.vue";
export default {
  name: "App",
  components: {
    Header,
    Slider,
    Offers,
    OffersSecond,
    OffersThird,
    InfoWrapper,
    Contact,
  },
  
  
};
</script>

<style>
html{
  width: 100%;
    height: 100%;
    margin: 0px;
    padding: 0px;
    overflow-x: hidden; 
    background-color:#0e1111;
    -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
    scroll-snap-type: y mandatory;
    

}
#app{
  
}
.snap {
  scroll-snap-align: start;
}
*{
  
  margin: 0px;
  box-sizing: border-box;
}
</style>
