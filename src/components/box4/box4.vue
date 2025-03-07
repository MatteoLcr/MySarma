<script setup>
import immagine_app from '../../assets/box4/immagine_app.png';
import { ArrowNarrowRightIcon } from '@heroicons/vue/solid';
</script>

<template>
    <div class="containerBox4 flex flex-col lg:flex-row justify-center items-center mt-25 lg:mt-0">
        <div class="flex flex-col justify-center items-start ">
            <h5 class="size48 lg:size72 ms-5 lg:ms-0">App</h5>
            <img class="block md:hidden mt-5 scale-85" :src="immagine_app" alt="">
            <p class="colorGray2 size24 ms-5 mt-8 lg:ms-0 lg:w-120 lg:my-15">
                Con l’app MySarma gestirai il tuo credito welfare e potrai accedere al catalogo dei Benefit e Servizi
                acquistabili.
            </p>
            <button class="flex justify-center items-center mt-10 ms-5 lg:mt-0 lg:ms-0">
                <ArrowNarrowRightIcon class="w-7 h-5 me-5 colorDarkBlue" />
                <p class="size16 colorDarkBlue">COMING SOON</p>
            </button>
        </div>
        <div class="hidden lg:block">
            <img :src="immagine_app" alt="">
        </div>
    </div>

</template>

<style scoped>
.containerBox4 {
    height: 800px;
}
</style>