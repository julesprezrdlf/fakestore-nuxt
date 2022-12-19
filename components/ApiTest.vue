<template>
  <div class="apite">
    {{ holaMundo }}
    <div class="allProducts" v-for="(product, id) in productsApi" :key="product.id">

          <p>{{ product.price}}</p>
          <p>{{ product.title}}</p>
          <p>{{ product.description}}</p>
        </div>
  </div>
</template>

<script>
import { assertOptionalIndexedAccessType } from "@babel/types";
import axios from "axios";
export default {
  data() {
    return {
      productsApi: [],
      holaMundo: "holaMUndoDesconocido",
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