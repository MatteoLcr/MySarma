<script setup>
import { ref } from "vue";
import { LoginIcon } from '@heroicons/vue/solid';

const btnBackground = ref("#ABE8DC");
const changeColor = () => {
    btnBackground.value = "#34BFA3";
};
const resetColor = () => {
    btnBackground.value = "#ABE8DC";
};
</script>

<template>
    <div class="flex relative">
        <button 
            class="btnGreen1 flex justify-center items-center relative z-10"
            @mouseenter="changeColor"
            @mouseleave="resetColor"
        >
            <LoginIcon class="w-4 h-4 me-1" />
            <p class="size14_2 colorDarkBlue">Accedi alla piattaforma</p>
        </button>
        <div 
            class="btnGreenUnder absolute" 
            :style="{ backgroundColor: btnBackground }"
        ></div>
    </div>
</template>

<style scoped>
.btnGreen1 {
    position: relative;
    height: 36px;
    width: 184px;
    border-radius: 10px;
    border: 2px solid #112340;
    z-index: 2;
}

.btnGreenUnder {
    position: absolute;
    height: 36px;
    width: 184px;
    top: 6px;
    left: 5px;
    border-radius: 10px;
    transition: background-color 0.2s ease-in-out;
    z-index: 1;
}
</style>
