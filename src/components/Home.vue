<template>
  <v-container>
    <v-row height="200px">
        <v-carousel>
          <v-carousel-item v-for="(item,i) in items" :key="i" :src="item.image">
            <v-row class="landing-text white--text lead">
              <h3 class="text-uppercase  font-weight-regular display-2">{{item.title}}</h3>
              <h5 class="text-capitalize font-weight-regular display-2">{{item.subtitle}}</h5>
              <p>{{item.details}}</p>
            </v-row>
          </v-carousel-item>
        </v-carousel>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'Home',
    
    data: () => ({
        items: [
          { 
            image: require("../assets/images/home.jpg"),
            title: "the best and finest of wine",
            subtitle: "good wine made from the best natural extracts",
            details:"The red-wine production process involves extraction of color and flavor components from the grape skin. Red wine is made from dark-colored grape varieties."
          }
        ]
    })
   
  }
</script>


<style scoped>
  .landing-text{
     font-size: 30px;   
    }
</style>

