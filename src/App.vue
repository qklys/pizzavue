<template>
  <div id="app">
   <h1>Parent: {{pizzaName}}</h1>
   <app-pizza v-bind:pizzaName='pizzaName' v-bind:pizzaPrice='pizzaPrice' v-bind:pizzaSize='pizzaSize'>
       

     <h1>Мы рады вам предложить!</h1>
     <h2 slot='n1'></h2>
   </app-pizza>
  </div>
</template>

<script>
import Pizza from './components/Pizza.vue'

export default {
  name: 'app',
  data(){
    return {
      pizzaName: 'Пицца от школы программистов',
      pizzaPrice: 600,
      pizzaSize: '60cm',
    }
  },
  components: {
    appPizza: Pizza
  } 
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
