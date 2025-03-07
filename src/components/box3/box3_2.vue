<script setup>
import { ArrowNarrowRightIcon } from '@heroicons/vue/solid';
import Guru_img from '../../assets/box3/Guru_img.png';
import Pianista_img from '../../assets/box3/Pianista_img.png';
import Servizi_img from '../../assets/box3/Servizi_img.png';
import Piattaforma_img from '../../assets/box3/Piattaforma_img.png';
</script>

<template>
    <div class="flex flex-col justify-center items-center mt-100">

        <h3 class="text-center size32 colorDarkBlue">Offriamo alle PMI</h3>
        <h3 class="text-center size32 colorDarkBlue">supporto nei seguenti </h3>
        <h3 class="text-center size32 colorDarkBlue">ambiti </h3>

        <div class="flex flex-col rounded-4xl mt-10" style="background-color: #283B6C; width: 95%;">
            <h3 class="text-white size48 text-center mt-8">Welfare Guru</h3>
            <img :src="Guru_img" alt="Welfare Guru" style="scale: 1;" />
            <button class="flex justify-center items-center size16 text-white mb-10">
                <ArrowNarrowRightIcon class="w-7 h-5 me-5" />
                SCOPRI DI PIU'
            </button>
        </div>

        <div class="flex flex-col rounded-4xl mt-10" style="background-color: #716ACA; width: 95%;">
            <h3 class="text-white size48 text-start ms-10 mt-8">Gestione del piano</h3>
            <img :src="Pianista_img" alt="Welfare Guru" style="scale: 1;" />
            <button class="flex justify-center items-center size16 text-white mb-10">
                <ArrowNarrowRightIcon class="w-7 h-5 me-5" />
                SCOPRI DI PIU'
            </button>
        </div>

        <div class="flex flex-col rounded-4xl mt-10" style="background-color: #426BD1; width: 95%;">
            <h3 class="text-white size48 text-start ms-10 mt-8">Soluzioni welfare esclusive</h3>
            <img :src="Piattaforma_img" alt="Welfare Guru" style="scale: 1;" />
            <button class="flex justify-center items-center size16 text-white mb-10 mt-8">
                <ArrowNarrowRightIcon class="w-7 h-5 me-5" />
                SCOPRI DI PIU'
            </button>
        </div>

        <div class="flex flex-col rounded-4xl mt-10" style="background-color: #299882; width: 95%;">
            <h3 class="text-white size48 text-start ms-10 mt-8">Piattaforma web dedicata</h3>
            <img :src="Servizi_img" alt="Welfare Guru" style="scale: 1;" />
            <button class="flex justify-center items-center size16 text-white mb-10">
                <ArrowNarrowRightIcon class="w-7 h-5 me-5" />
                SCOPRI DI PIU'
            </button>
        </div>

    </div>

</template>

<style scoped></style>
