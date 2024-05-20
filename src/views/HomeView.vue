
<template>
  <div class="home">
   <div class="count">
     {{storeCounter.count}}
   </div>

   <div class="button">
    <button @click="storeCounter.decreaseCount">-</button>
    <button @click="storeCounter.increaseCount">+</button>
   </div>
   <hr>

   <div>
    This counter is: {{ storeCounter.oddOrEven}}
   </div>

   <hr>

   <div>
       <h4>Edit Counter:</h4>
       <input
       v-model="storeCounter.count"
        type="number">
   </div>
  </div>
  
</template>

<script setup>
import {useCounterStore} from "@/stores/counter"

const storeCounter = useCounterStore()
</script>

<style>
.count{
  font-size: 60px;
  margin: 20px;
}

.button button{
  font-size: 40px;
  margin: 10px;
  background-color: #04AA6D;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}
</style>
