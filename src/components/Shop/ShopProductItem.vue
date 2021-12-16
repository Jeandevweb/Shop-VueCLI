<template>
  <div class="w-25 p-3 product-container d-flex flex-column">
    <div d-flexflex-row justify-content-center>
      <img v-bind:src="product.img" style="height:150px; width:100% " />
    </div>
    <div>
      <h3>{{ product.title }}</h3>
      <hr>
    </div>
    <div>
      <p> {{ product.description }}</p>
    </div>
    <div>
      <span>{{ product.price }}</span>
      <button class="btn btn-primary btn-sm float-right">Commandez Vos Produits</button>
    </div>
  </div>
</template>

<script>





export default {
  data() {
    return {
      product: {
        img: 'https://www.apple.com/ac/structured-data/images/open_graph_logo.png?202111120425',
        title: 'Apple',
        description:"Apple [ˈæpəl] est une entreprise multinationale américaine qui crée et commercialise des produits électroniques grand public, des ordinateurs personnels et des logiciels",
        price: "1500€"
      }
    };
  }

}
</script>

<style>
.product-container{
   height: 400px; 
  }
p {
  font-size: 12px;

}

</style>