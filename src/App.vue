<template>
  <v-app id="app">
    <v-app-bar
      app
      color="primary"
      dark
      dense
    >
      <div class="d-flex align-center">
        <v-btn text >
           <span class="ml-2">Dtoolz Wine Cellar</span>
        </v-btn>
      </div>

      <v-spacer></v-spacer>
      <v-btn text >
        <v-icon>mdi-bottle-wine-outline</v-icon>
        <span class="mr-2">Products</span>
      </v-btn>
      <v-btn text >
        <span class="mr-2">Cart</span>
        <v-icon>mdi-cart-outline</v-icon>
      </v-btn>
      <v-btn text >
        <span class="mr-2">About</span>
      </v-btn>
    </v-app-bar>

    <v-content>
      <Home/>
    </v-content>
  </v-app>
</template>

<script>
import Home from './components/Home';

export default {
  name: 'App',

  components: {
    Home,
  },

  data: () => ({
    //
  }),
};
</script>


<style>
 #app{
   font-family: 'Cormorant', serif !important;
 }
</style>