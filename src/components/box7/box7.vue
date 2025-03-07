<script setup>
import { BadgeCheckIcon } from '@heroicons/vue/solid';
import { InformationCircleIcon } from '@heroicons/vue/solid'
import smallBox from '../pricing/smallBox.vue';
import largeBox from '../pricing/largeBox.vue';

</script>

<template>

    <div class=" flex justify-center items-center ">
        <div class="box7Container lg:max-w-[861px] flex flex-col justify-center items-center">
            <!-- BLOCCO TITOLI -->
            <div class="flex flex-col justify-center items-center mt-15 mb-15 lg:mb-0 lg:p-30lg:mt-0">
                <h5 class="size32 lg:size48 colorDarkBlue text-center px-15 py-5 lg:px-0 lg:py-0">Attiva il tuo piano Go oppure Pro</h5>
                <p class="size24 colorGray2 text-center px-10 mb-10 lg:px-0 ">Scegli se attiavre subito il Piano Go oppure richiedere
                    un preventivo per il Piano Pro al nostro consulente
                </p>
            </div>

            <div class="flex flex-col justify-between lg:w-[861px] lg:flex-row">
                <!-- BOX DI SINISTRA -->
                <smallBox />
                <!-- BOX DI DESTRA -->
                <largeBox />
            </div>
        </div>
    </div>

</template>

<style scoped>

</style>