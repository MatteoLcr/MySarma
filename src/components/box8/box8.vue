<script setup>
import { ArrowNarrowRightIcon } from '@heroicons/vue/solid';
import Omninext_icon from '../../assets/box8/Omninext_icon.png';
</script>

<template>

    <div class="lg:w-full flex-col lg:flex-row lg:justify-center lg:items-center mt-30 lg:mt-50 px-5 lg:px-0">
        
        <div class="box8Container  lg:max-w-[1440px] lg:max-h-[362px] flex flex-col lg:flex-row lg:justify-evenly items-center rounded-4xl py-10 px-5">
            <img :src="Omninext_icon" alt="" class="lg:w-[239px] h-[239px] mb-5 lg:mb-0">
            
            <div class="lg:w-[557px]">
                <h3 class="size32 lg:size48 colorBlue1">Facciamo parte</h3>
                <h3 class="size32 lg:size48 colorBlue1">di un grande gruppo!</h3>
                <p class="size16 lg:size18_2 colorGray2 hidden lg:block">Il Gruppo Omninext è costituito da aziende altamente specializzate interconnesse tra loro, che
                    permettono di ricoprire diversi settori industriali per necessità di Business personalizzate.
                </p>
                <button class="flex justify-center items-center mt-8">
                    <ArrowNarrowRightIcon class="w-7 h-5 me-5 colorBlue1" />
                    <p class="size16 colorBlue1">SCOPRI DI PIU</p>
                </button>
            </div>
        </div>

    </div>
</template>

<style scoped>
.box8Container {
    /* width: 1440px; */
    border: 1px solid #2B50B0;
}
</style>