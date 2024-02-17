<template>
  <div>
  <select name="" id="">
    <option v-for="items in cpus"
    :key="items.name"> {{ items.name }} - ${{ items.price }}</option>
  </select>
  </div>
</template>

<script>
import Greet from './components/GreetPpl.vue'

export default {
  name: 'App',
  components: {
    Greet,
  },
  data() {
    return {
      cpus: [
        { "name": "AMD Ryzen 7 7800X3D", "price": 385.87, "core_count": 8, "core_clock": 4.2, "boost_clock": 5, "tdp": 120, "graphics": "Radeon", "smt": true }, { "name": "AMD Ryzen 5 5600X", "price": 159.68, "core_count": 6, "core_clock": 3.7, "boost_clock": 4.6, "tdp": 65, "graphics": null, "smt": true }, { "name": "AMD Ryzen 5 7600X", "price": 228, "core_count": 6, "core_clock": 4.7, "boost_clock": 5.3, "tdp": 105, "graphics": "Radeon", "smt": true }, { "name": "AMD Ryzen 5 7600", "price": 218.99, "core_count": 6, "core_clock": 3.8, "boost_clock": 5.1, "tdp": 65, "graphics": "Radeon", "smt": true }, { "name": "Intel Core i9-14900K", "price": 548.99, "core_count": 24, "core_clock": 3.2, "boost_clock": 6, "tdp": 125, "graphics": "Intel UHD Graphics 770", "smt": true }, { "name": "Intel Core i7-13700K", "price": 370.99, "core_count": 16, "core_clock": 3.4, "boost_clock": 5.4, "tdp": 125, "graphics": "Intel UHD Graphics 770", "smt": true }, { "name": "AMD Ryzen 5 5600", "price": 131.99, "core_count": 6, "core_clock": 3.5, "boost_clock": 4.4, "tdp": 65, "graphics": null, "smt": true }, { "name": "AMD Ryzen 7 5800X", "price": 218.36, "core_count": 8, "core_clock": 3.8, "boost_clock": 4.7, "tdp": 105, "graphics": null, "smt": true }, { "name": "Intel Core i5-12400F", "price": 148.99, "core_count": 6, "core_clock": 2.5, "boost_clock": 4.4, "tdp": 65, "graphics": null, "smt": true }, { "name": "AMD Ryzen 5 5500", "price": 99, "core_count": 6, "core_clock": 3.6, "boost_clock": 4.2, "tdp": 65, "graphics": null, "smt": true }, { "name": "AMD Ryzen 5 3600", "price": 108.9, "core_count": 6, "core_clock": 3.6, "boost_clock": 4.2, "tdp": 65, "graphics": null, "smt": true }, { "name": "Intel Core i7-14700K", "price": 399.78, "core_count": 20, "core_clock": 3.4, "boost_clock": 5.6, "tdp": 125, "graphics": "Intel UHD Graphics 770", "smt": true }, { "name": "Intel Core i5-12600K", "price": 212.99, "core_count": 10, "core_clock": 3.7, "boost_clock": 4.9, "tdp": 125, "graphics": "Intel UHD Graphics 770", "smt": true }, { "name": "AMD Ryzen 7 7700X", "price": 312.49, "core_count": 8, "core_clock": 4.5, "boost_clock": 5.4, "tdp": 105, "graphics": "Radeon", "smt": true }, { "name": "AMD Ryzen 9 7950X3D", "price": 619, "core_count": 16, "core_clock": 4.2, "boost_clock": 5.7, "tdp": 120, "graphics": "Radeon", "smt": true }, { "name": "Intel Core i5-13600K", "price": 293.99, "core_count": 14, "core_clock": 3.5, "boost_clock": 5.1, "tdp": 125, "graphics": "Intel UHD Graphics 770", "smt": true }, { "name": "AMD Ryzen 7 5700X", "price": 180.59, "core_count": 8, "core_clock": 3.4, "boost_clock": 4.6, "tdp": 65, "graphics": null, "smt": true }, { "name": "Intel Core i7-12700K", "price": 280.38, "core_count": 12, "core_clock": 3.6, "boost_clock": 5, "tdp": 125, "graphics": "Intel UHD Graphics 770", "smt": true }, { "name": "AMD Ryzen 7 5800X3D", "price": 305.11, "core_count": 8, "core_clock": 3.4, "boost_clock": 4.5, "tdp": 105, "graphics": null, "smt": true }, { "name": "AMD Ryzen 5 5600G", "price": 137.97, "core_count": 6, "core_clock": 3.9, "boost_clock": 4.4, "tdp": 65, "graphics": "Radeon Vega 7", "smt": true }, { "name": "Intel Core i3-12100F", "price": 98.98, "core_count": 4, "core_clock": 3.3, "boost_clock": 4.3, "tdp": 58, "graphics": null, "smt": true }, { "name": "AMD Ryzen 9 7900X", "price": 386.99, "core_count": 12, "core_clock": 4.7, "boost_clock": 5.6, "tdp": 170, "graphics": "Radeon", "smt": true }, { "name": "AMD Ryzen 9 5900X", "price": 298.99, "core_count": 12, "core_clock": 3.7, "boost_clock": 4.8, "tdp": 105, "graphics": null, "smt": true }, { "name": "Intel Core i5-12600KF", "price": 183.89, "core_count": 10, "core_clock": 3.7, "boost_clock": 4.9, "tdp": 125, "graphics": null, "smt": true }, { "name": "AMD Threadripper 3990X", "price": 4355, "core_count": 64, "core_clock": 2.9, "boost_clock": 4.3, "tdp": 280, "graphics": null, "smt": true }, { "name": "Intel Core i5-13400F", "price": 203.99, "core_count": 10, "core_clock": 2.5, "boost_clock": 4.6, "tdp": 65, "graphics": null, "smt": true }, { "name": "Intel Core i7-14700KF", "price": 369.99, "core_count": 20, "core_clock": 3.4, "boost_clock": 5.6, "tdp": 125, "graphics": null, "smt": true }, { "name": "Intel Core i9-13900K", "price": 524.99, "core_count": 24, "core_clock": 3, "boost_clock": 5.8, "tdp": 125, "graphics": "Intel UHD Graphics 770", "smt": true }, { "name": "AMD Ryzen 5 4500", "price": 79, "core_count": 6, "core_clock": 3.6, "boost_clock": 4.1, "tdp": 65, "graphics": null, "smt": true }, 
      ]
    }
  }
} 
</script>

<style scoped>
#app {
  font-family: 'Times New Roman', Times, serif;
  float: left;
}
</style>