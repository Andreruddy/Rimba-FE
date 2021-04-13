<template>
  <div class="home">
    <Header/>
    <HeroRimba/>
    <ProductsItem/>
    <Footer/>

    <!-- Header End -->
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import HeroRimba from '@/components/HeroRimba.vue'
import ProductsItem from '@/components/ProductsItem.vue'
import Footer from '@/components/Footer.vue'



export default {
  name: 'Home',
  components: {
    Header,
    HeroRimba,
    ProductsItem,
    Footer
  }
}
</script>
