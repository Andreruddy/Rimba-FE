<template>
    <section class="hero-section">
    <carousel class="hero-items" autoplay="true" :nav="false" items="1">
      <div
        class="single-hero-items set-bg"
        style="background-image: url('/img/tools.jpg')"
      >
        <!-- <div class="container">
          <div class="row">
            <div class="col-lg-5">
              <span>Bag,kids</span>
              <h1>Black friday</h1>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
                eiusmod tempor incididunt ut labore et dolore
              </p>
              <a href="#" class="primary-btn">Shop Now</a>
            </div>
          </div>
        </div> -->
      </div>
      <div
        class="single-hero-items set-bg"
        style="background-image: url('/img/tools-2.jpg')"
      >
        <!-- <div class="container">
          <div class="row">
            <div class="col-lg-5">
              <span>Bag,kids</span>
              <h1>Black friday</h1>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
                eiusmod tempor incididunt ut labore et dolore
              </p>
              <a href="#" class="primary-btn">Shop Now</a>
            </div>
          </div>
        </div> -->
      </div>
      <div
        class="single-hero-items set-bg"
        style="background-image: url('/img/tools-3.jpg')"
      >
        <!-- <div class="container">
          <div class="row">
            <div class="col-lg-5">
              <span>Bag,kids</span>
              <h1>Black friday</h1>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
                eiusmod tempor incididunt ut labore et dolore
              </p>
              <a href="#" class="primary-btn">Shop Now</a>
            </div>
          </div>
        </div> -->
      </div>
    </carousel>
  </section>
</template>
<script>
import carousel from 'vue-owl-carousel';

export default {
    name:'HeroRimba',
    components: {
        carousel
    }
}
</script>