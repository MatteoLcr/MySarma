<script setup>
import 'vue3-carousel/dist/carousel.css';

import navbar from './components/navbar/navbar.vue';
import box1 from './components/box1/box1.vue';
import box2 from './components/box2/box2.vue';
import box3 from './components/box3/box3.vue';
import box3_2 from './components/box3/box3_2.vue';
import box4 from './components/box4/box4.vue';
import box5 from './components/box5/box5.vue';
import box6 from './components/box6/box6.vue';
import box7 from './components/box7/box7.vue';
import box8 from './components/box8/box8.vue';
import box9 from './components/box9/box9.vue';
import box10 from './components/box10/box10.vue';
import box11 from './components/box11/box11.vue';
import box11_2 from './components/box11/box11_2.vue';

</script>

<template>

  <navbar />
  <box1 />
  <box2 class="hidden lg:block" />
  <box3 class="hidden lg:block"/>
  <box3_2 class="block lg:hidden"/>
  <box4 />
  <box5 />
  <box6 />
  <box7 />
  <box8 />
  <box9 />
  <box10 />
  <box11 class="hidden lg:block" />
  <box11_2 class="block lg:hidden"/>

</template>




<style scoped></style>
