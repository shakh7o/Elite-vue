<script setup>
import 'primeicons/primeicons.css';
import myHeader from './components/app/myHeader.vue';
import myFooter from './components/app/myfooter.vue';
import cardVue from './components/app/ui/card.vue';
</script>

<template>
  <div>
    <my-header/>  
    <card-vue />
    <main class="main">
      <RouterView />
    </main>
    <myFooter />
  </div>
</template>

<style lang="scss" scoped>

</style>

