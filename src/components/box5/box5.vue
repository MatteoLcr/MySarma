<script setup>
import Mano from '../../assets/box5/Mano.png';
import Calamita from '../../assets/box5/Calamita.png';
import Risparmio from '../../assets/box5/Risparmio.png';
import Successo from '../../assets/box5/Successo.png';
</script>

<template>
    <div class="box5Container mx-auto flex flex-col justify-between items-center">
      <!-- Titolo -->
      <div class="flex flex-col justify-center items-center mb-10 mt-40 lg:mb-25 px-5 lg:mt-0 text-center lg:text-start lg:px-0">
        <h3 class="size48 lg:size72 colorDarkBlue">Welfare aziendale?</h3>
        <p class="size24 colorGray2">Te lo diciamo noi se non lo sai</p>
      </div>
  

      <div class="lg:grid lg:grid-cols-4 lg:gap-10 lg:mt-10 lg:max-w-[1440px] w-full flex flex-col mt-0 ">
   
        <div class="flex flex-col lg:justify-start items-center text-center bg-white p-6 mt-10 lg:mt-0 ">
          <img class="h-28 mb-10" :src="Mano" alt="">
          <h5 class="size18 colorGray1">Cos’è il Welfare Aziendale?</h5>
          <p class="size18_2 colorGray1">
            Tutti ne parlano ma pochi conoscono il suo potenziale.
          </p>
          <button class="itemBtnBox5 size18_3 mt-4">Scopri di più</button>
        </div>
  
        <!-- Item 2 -->
        <div class="flex flex-col lg:justify-start items-center text-center bg-white p-6 mt-10 lg:mt-0">
          <img class="h-28 mb-10" :src="Calamita" alt="">
          <h5 class="size18 colorGray1">Come posso attrarre?</h5>
          <p class="size18_2 colorGray1">
            Fidelizza e attrai nuovi talenti con un piano welfare mirato.
          </p>
          <button class="itemBtnBox5 size18_3 mt-4">Scopri di più</button>
        </div>
  
        <!-- Item 3 -->
        <div class="flex flex-col lg:justify-start items-center text-center bg-white p-6 mt-10 lg:mt-0">
          <img class="h-28 mb-10" :src="Risparmio" alt="">
          <h5 class="size18 colorGray1">Normative e vantaggi fiscali</h5>
          <p class="size18_2 colorGray1">
            Risparmiare è facile grazie al tuo nuovo piano welfare.
          </p>
          <button class="itemBtnBox5 size18_3 mt-4">Scopri di più</button>
        </div>
  
        <!-- Item 4 -->
        <div class="flex flex-col lg:justify-start items-center text-center bg-white p-6 mt-10 lg:mt-0">
          <img class="h-28 mb-10" :src="Successo" alt="">
          <h5 class="size18 colorGray1">Storie attrattive</h5>
          <p class="size18_2 colorGray1">
            Ascolta le testimonianze di chi ha migliorato il proprio stile di vita.
          </p>
          <button class="itemBtnBox5 size18_3 mt-4">Scopri di più</button>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  .box5Container {
    max-width: 1440px;
  }

  .itemBtnBox5{
    height: 50px;
    width: 165px;
    border: 2px solid #112340;
    border-radius: 10px;
  }
  
 
  </style>
  