<script setup>
import { BadgeCheckIcon } from '@heroicons/vue/solid';
import { InformationCircleIcon } from '@heroicons/vue/solid'
import { ref } from "vue";

const btnBackground = ref("#FFFFFF");
const changeColor = () => {
    btnBackground.value = "#A1B5E8";
};
const resetColor = () => {
    btnBackground.value = "#FFFFFF";
};
</script>

<template>
    <div class="h-[674px] w-[341px] ms-2 lg:ms-0">
        <div class="sxBox h-[654px] w-[391px] flex flex-col justify-center items-center rounded-3xl">

            <div class="flex flex-col justify-center items-center">
                <h3 class="size24_3 colorBlue1">Piano GO!</h3>
                <p class="size12 colorBlue2 ">a partire da</p>
                <div class="flex">
                    <h4 class="colorDarkBlue size60 font-bold">€</h4>
                    <h4 class="colorDarkBlue size60 font-bold">12</h4>
                    <div class="flex flex-col justify-center items-center">
                        <p class="colorDarkBlue font-bold text-4xl">,50</p>
                        <p class="colorBlue2 size12">+IVA</p>
                    </div>
                </div>
                <div class="flex justify-center items-center">
                    <p class="colorBlue2 size16 me-2">all'anno / per utente </p>
                    <InformationCircleIcon class="w-4 h-4 colorBlue2" />
                </div>
            </div>

            <div class="divider my-4"></div>

            <div class="flex flex-col justify-center">
                <div class="flex justify-start items-center">
                    <BadgeCheckIcon class="checkIcon h-5.5 me-2" />
                    <h5 class="colorDarkBlue my-2 size16"> Utenti illimitati</h5>
                </div>
                <div class="flex justify-start items-center">
                    <BadgeCheckIcon class="checkIcon h-5.5 me-2" />
                    <h5 class="colorDarkBlue my-2 size16"> Piattaforma MySarma</h5>
                </div>
                <div class="flex justify-start items-center">
                    <BadgeCheckIcon class="checkIcon h-5.5 me-2" />
                    <h5 class="colorDarkBlue my-2 size16"> Gestione del contratto
                        online</h5>
                </div>
                <div class="flex justify-start items-center">
                    <BadgeCheckIcon class="checkIcon h-5.5 me-2" />
                    <h5 class="colorDarkBlue my-2 size16"> MySarma Welfare Card
                        (fino a 258 €)</h5>
                </div>
                <div class="flex justify-start items-center">
                    <BadgeCheckIcon class="checkIcon h-5.5 me-2" />
                    <h5 class="colorDarkBlue my-2 size16"> Importi personalizzabili
                        online</h5>
                </div>
                <div class="flex justify-start items-center">
                    <BadgeCheckIcon class="checkIcon h-5.5 me-2" />
                    <h5 class="colorDarkBlue my-2 size16"> Sconti e Coupon</h5>
                </div>
            </div>

            <button class="btnWhiteLarge my-5" @mouseenter="changeColor" @mouseleave="resetColor">Attiva Piano GO!</button>
            <div class="btnWhiteLargeUnder absolute" :style="{ backgroundColor: btnBackground }"></div>

            <div class="flex flex-col justify-center items-center">
                <p class="size16 colorGray2">Vuoi maggiorni informazioni sul piano?</p>
                <p class="colorBlue2 size16_2 underline">Scopri di più</p>
            </div>
        </div>
        <div class="boxUnder h-[654px] w-[391px] rounded-3xl"></div>
    </div>
</template>

<style scoped>
.sxBox {
    border: 2px solid #112340;
    z-index: 3;
}

.boxUnder {
    position: relative;
    bottom: 645px;
    left: 10px;
    background-color: #E6ECF9;
    z-index: -1;
}

.divider {
    width: 80%;
    border: 2px solid #112340;
    border-radius: 50px;
}
</style>