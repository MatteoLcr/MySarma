<script setup>
import { ref } from "vue";
import box1_bg from "../../assets/box1_bg.png";
import pianoImg from "../../assets/pianoImg.png";
import logo_mysarma from "../../assets/logo_mysarma.png";
import box1Pricing from "../pricing/box1Pricing.vue";
import box1PricingSmall from "../pricing/box1PricingSmall.vue";


const isVisible = ref(true);
const hideDiv = () => {
    isVisible.value = false;
};

</script>

<template>
    <div class="box1Container flex flex-col lg:flex-row justify-center items-center"
        :style="{ backgroundImage: `url(${box1_bg})` }">

        <div class="flex flex-col mt-100 lg:mt-0 lg:me-20 w-80 lg:w-150">
            <h2 class="size48 lg:[size72] text-white mb-10">Il Welfare aziendale a portata di PMI</h2>
            <p class="size24 text-white mb-10">MySarma nasce con l'obiettivo di supportare le aziende a rispondere
                concretamente ai
                bisogni di welfare
                dei propri dipendenti e collaboratori.
            </p>

            <div v-if="isVisible" class="box1interactiveItem hidden lg:flex items-center p-3">
                <img :src="pianoImg" alt="" class="h-15 w-15 me-3">
                <p class="colorBlue2 size16">Da oggi puoi attivare il tuo piano welfare direttamente online ed in pochi
                    semplici passaggi grazie
                    al <span class="colorBlue1 font-bold">Piano GO!</span>
                </p>
                <XIcon @click="hideDiv" class="w-5 h-5 mb-10 colorBlue1" />
            </div>
            <p class="block lg:hidden size16 text-white mb-5">
                Da oggi puoi attivare il tuo piano welfare direttamente online ed in pochi semplici passaggi grazie al
                Piano GO!
            </p>
        </div>
        <box1Pricing class="hidden md:block"/>
        <box1PricingSmall class="block md:hidden"/>
    </div>
</template>



<style scoped>
.box1Container {
    position: relative;
    height: 90vh;
    width: 100%;
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    padding: 30px;
    z-index: 0;
}

.box1interactiveItem {
    background-color: rgba(255, 255, 255, 0.688);
    border-radius: 15px;
}
</style>