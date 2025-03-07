<script setup>
import { ref } from "vue";
import { LoginIcon } from '@heroicons/vue/solid';
import menuTendina from "./menuTendina.vue";
import logo_mysarma from "../../assets/logo_mysarma.png";
import Logo from "../../assets/Logo.png";
import Accedi from "../../assets/Accedi.png";
import greenBtn from "../buttons/greenBtn.vue";

const isOpen = ref(false);
</script>


<template>
    <nav class="p-4 lg:py-3 lg:px-30">
        <div class="container flex justify-between items-center">
            <div class="flex items-center">
                <img :src="Logo" alt="" class="h-10 me-2">
            </div>

            <!-- Menu per desktop -->
            <div class="navBoxServizi hidden md:flex space-x-15 mx-10">
                <a href="#" class="colorBlue1 hover:underline">Welfare aziendale</a>
                <a href="#" class="colorBlue1 hover:underline">Chi siamo</a>
                <a href="#" class="colorBlue1 hover:underline">I nostri servizi</a>
                <a href="#" class="colorBlue1 hover:underline">Soluzioni welfare</a>
                <a href="#" class="colorBlue1 hover:underline">Blog</a>
            </div>

            <button class="ms-15 block lg:hidden">
                <img class="h-6" :src="Accedi" alt="">
            </button>
            <greenBtn class="hidden lg:block " />

            <!-- Bottone per mobile -->
            <button @click="isOpen = !isOpen" class="md:hidden text-blue">
                ☰
            </button>
        </div>

        <!-- Menu per mobile -->
        <div v-if="isOpen" class="md:hidden flex flex-col p-4">
            <menuTendina />
            <!-- <a href="#" class="colorBlue1 hover:underline">Welfare aziendale</a>
            <a href="#" class="colorBlue1 hover:underline">Chi siamo</a>
            <a href="#" class="colorBlue1 hover:underline">I nostri servizi</a>
            <a href="#" class="colorBlue1 hover:underline">Soluzioni welfare</a>
            <a href="#" class="colorBlue1 hover:underline">Blog</a> -->
        </div>
    </nav>
</template>


<style>
/* .navBoxServizi a {
    font-size: 14px;
    font-weight: 700;
} */
</style>