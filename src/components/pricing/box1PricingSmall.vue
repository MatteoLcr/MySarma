<script setup>
import { BadgeCheckIcon } from '@heroicons/vue/solid';
import { XIcon } from "@heroicons/vue/solid"
import { ref } from "vue";
import { Disclosure, DisclosureButton, DisclosurePanel } from '@headlessui/vue'

const value = ref('')
const toggleDisclosure = () => {
    value.value = value.value === 'open' ? 'closed' : 'open';  // Alterna lo stato
};

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
        <div class="dxBox flex flex-col justify-center items-center p-7 mb-30">
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

            <div class="answare">
                <Disclosure v-slot="{ open }">
                    <DisclosureButton @click="toggleDisclosure" class=" flex justify-center w-full py-2 text-left">
                        <svg :class="open ? 'rotate-180' : ''" class="w-5 h-5 transition-transform" viewBox="0 0 20 20"
                            fill="currentColor">
                            <path fill-rule="evenodd"
                                d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                                clip-rule="evenodd" />
                        </svg>
                    </DisclosureButton>
                    <DisclosurePanel class="p-4 bg-transparent">
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
                    </DisclosurePanel>
                </Disclosure>
            </div>

            <div>
                <button class="btnWhite1 my-5  flex justify-center items-center relative z-10" @mouseenter="changeColor"
                    @mouseleave="resetColor">Attiva Piano GO!</button>
                 <div :class="value === 'open' ? 'btnWhite1Under' : 'btnWhite1UnderSmall'" :style="{ backgroundColor: btnBackground }"></div>
            </div>
            <div class="flex flex-col">
                <p>vuoi maggiorni informazioni sul piano?</p>
                <p>Scopri di più</p>
            </div>

        </div>
        <div :class="value === 'open' ? 'dxBoxUnder2' : 'dxBoxUnder2Close'"></div>

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
    top: 120px;
    right: 200px;
    z-index: 1;
}

.dxBoxUnder2 {
    width: 370px;
    height: 700px;
    background-color: #E6ECF9;
    border-radius: 15px;
    position: absolute;
    top: 520px;
    right: 20px;
    z-index: 1;
}

.dxBoxUnder2Close {
    width: 315px;
    height: 400px;
    background-color: #E6ECF9;
    border-radius: 15px;
    position: absolute;
    top: 670px;
    right: 50px;
    z-index: 1;
}

.divider {
    height: 3px;
    width: 100%;
    background-color: #112340;
    border-radius: 50px;
}

.btnWhite1 {
    position: relative;
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
    position: absolute;
    width: 243px;
    height: 50px;
    border-radius: 10px;
    bottom: 80px;
    left: 68px;
    z-index: 1;
    transition: background-color 0.2s ease-in-out;
}

.btnWhite1UnderSmall {
    position: absolute;
    width: 243px;
    height: 50px;
    border-radius: 10px;
    bottom: 80px;
    left: 40px;
    z-index: 1;
    transition: background-color 0.2s ease-in-out;
}
</style>