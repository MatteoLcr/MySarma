<script setup>
import { BadgeCheckIcon } from '@heroicons/vue/solid';
import { XIcon } from "@heroicons/vue/solid"
import { ref } from "vue";

const btnBackground = ref("#E6ECF9");
const changeColor = () => {
    btnBackground.value = "#A1B5E8";
};
const resetColor = () => {
    btnBackground.value = "#E6ECF9";
};

</script>

<template>
    <div>
        <div class="dxBox flex flex-col justify-center items-center p-7">
            <div class="flex flex-col justify-center items-center">
                <h3 class="size24_3 colorBlue1">Piano GO!</h3>
                <p class="colorBlue2 size12">a partire da</p>
                <div class="flex">
                    <h4 class="colorDarkBlue text-7xl font-bold">€</h4>
                    <h4 class="colorDarkBlue text-7xl font-bold">12</h4>
                    <div class="flex flex-col justify-center items-center">
                        <p class="colorDarkBlue font-bold text-4xl">,50</p>
                        <p class="colorBlue2 size12">+IVA</p>
                    </div>
                </div>
                <p class="colorBlue2 size16">all'anno / per utente <span>i</span></p>
            </div>
            <div class="divider my-4"></div>
            <div class="flex flex-col list">
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

            <div>
                <button class="btnWhite1 my-5  flex justify-center items-center relative z-10" @mouseenter="changeColor"
                    @mouseleave="resetColor"
                    >Attiva Piano GO!</button>
                <div class="btnWhite1Under absolute" :style="{ backgroundColor: btnBackground }"></div>
            </div>
            <div class="flex flex-col">
                <p>vuoi maggiorni informazioni sul piano?</p>
                <p>Scopri di più</p>
            </div>

        </div>
        <div class="dxBoxUnder hidden md:block"></div>
        <!-- <div class="dxBoxUnder2 block md:hidden "></div> -->
    </div>
</template>

<style scoped>
.dxBox {
    border: 2px solid #112340;
    border-radius: 15px;
    z-index: 2;
    padding: 20px;
    position: relative;
}

.dxBoxUnder {
    width: 340px;
    height: 608px;
    background-color: #E6ECF9;
    border-radius: 15px;
    position: absolute;
    top: 122px;
    right: 203px;
    z-index: 1;
}

/* .dxBoxUnder2 {
    width: 340px;
    height: 608px;
    background-color: #E6ECF9;
    border-radius: 15px;
    position: absolute;
    top: 630px;
    right: 35px;
    z-index: 1;
} */

.divider {
    height: 3px;
    width: 100%;
    background-color: #112340;
    border-radius: 50px;
}

.btnWhite1 {
    border: 2px solid #112340;
    border-radius: 10px;
    width: 243px;
    height: 50px;
    color: #112340;
    font-size: 18px;
    font-weight: 700;
    z-index: 2;
}

.btnWhite1Under {
    width: 243px;
    height: 50px;
    border-radius: 10px;
    bottom: 83px;
    left: 53px;
    z-index: 1;
    transition: background-color 0.2s ease-in-out;
}

</style>