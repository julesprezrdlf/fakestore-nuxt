<template>
  <div class="apite">
    {{ holaMundo }}
    <div class="allProducts" v-for="(product, id) in productsApi" :key="product.id">

          <p>{{ product.price}}</p>
          <p>{{ product.title}}</p>
          <p>{{ product.description}}</p>


<!-- the card  -->


          <div class="cardHolder-container">
    <div class="cardHolder-wrap">
      <div class="cardHolder">
        <div class="cardHolder-nameTag">
          <b-row>
            <b-col cols="9" class="cardHolder-titleTag"
              >{{ product.title}}</b-col
            >
          </b-row>
        </div>
        <!-- product goes here -->
        <img v-bind:src="product.image"/>


        <!-- button I HAVE TO MAKE THIS AS A COMPONENT -->
        <div class="cardHolder-buttonsContainer">
          <button class="button-49" role="button">MORE INFO</button>
        </div>
      </div>
    </div>
  </div>
        </div>
  </div>
</template>

<script>

import axios from "axios";
export default {
  data() {
    return {
      productsApi: [],

    };
  },

  methods: {
    async getProducts () {
        const response = await axios.get ('https://fakestoreapi.com/products')
        this.productsApi = response.data
        console.log(this.productsApi)
    }
  },
  created(){
    this.getProducts()
  }
};
</script>

<style>
</style>