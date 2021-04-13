<template>
    <section class="women-banner spad">
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-12 mt-5" v-if="items.length > 0">
          <carousel
            class="product-slider"
            :autoplay="true"
            :nav="false"
            :loop="false"
            :dots="false"
          >
            <div class="product-item" v-for="items in items" v-bind:key="items.id">
              <div class="pi-pic">
                <img v-bind:src="items.image" alt=""/>
                <ul>
                  <li class="w-icon active">
                    <a href="#"><i class="icon_bag_alt"></i></a>
                  </li>
                  <li class="quick-view">
                    <router-link v-bind:to="'/product'">+ Quick View</router-link>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <a href="#">
                  <h5>{{items.nama_item}}</h5>
                </a>
                <div class="product-price">
                  Rp. {{items.harga_satuan}}
                  <span>Rp. 34000</span>
                </div>
              </div>
            </div>
           
          </carousel>
        </div>
        <div class="col-lg-12" v-else> 
          Items belum tersedia
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import carousel from 'vue-owl-carousel';
import axios from 'axios';
export default {
    name:'ProductsItem',
    components: {
        carousel
    },
    data(){
      return {
        items:[]
      };
    },
    mounted() {
      axios
      .get("http://127.0.0.1:8001/api/items")
      .then(res=>(this.items = res.data.data))
      .catch(err => console.log(err));
    }

}
</script>
<style scoped>
.product-item {
  margin-right: 25px;
}
.product-item .pi-pic img {
  min-width: 30%;
  max-height: 300px;
}
</style>