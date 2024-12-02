<template>
  <q-page class="flex flex-center text-black">
    <div class="row">
      <q-input 
      v-model="data.name"
      input-class="text-center text-h5 text-black"
      color="teal"
      placeholder="counter" 
      filled />
    </div>  
    <div class="rows full-width items-center">
      <div class="col text-center">
        <q-btn
          icon="remove" 
          size="xl"
        round 
        />
      </div>
      <div class="col text-center text-h2">
        {{ data.counter }}
      </div>
      <div class="col text-center">
        <q-btn
          icon="add_circle_outline" 
          size="xl"
        round 
        />
      </div>
    </div>
    <div class="row">
      <q-btn
          icon="resart_alt" 
          size="xl"
        round 
        />
    </div>
  </q-page>
</template>

<style scoped>
.q-page{
  max-width: 700px;
  margin: 0 auto;

}
</style>

<script setup>

import { reactive } from 'vue';
const data=reactive({
  counter: 10,
  name:'asdfasd'
})


</script>
