<template>
  <SideNav />
  <NavBar />
  <NavBar2 />
  <NavBar3 />
  <NavBar4 />
  <ProductTop />
  <Productarea1 />
</template>

<script setup>
import NavBar from './components/NavBar.vue'
import NavBar2 from './components/NavBar2.vue';
import NavBar3 from './components/NavBar3.vue';
import NavBar4 from './components/NavBar4.vue';
import Productarea1 from './components/Productarea1.vue';
import ProductTop from './components/ProductTop.vue';
import SideNav from './components/SideNav.vue';
</script>

<style>
html, body, #app {
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
}
</style>
