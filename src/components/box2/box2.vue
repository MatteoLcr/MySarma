<script setup>

import Guru_box2 from '../../assets/Guru_box2.png';
import Piano_box2 from '../../assets/Piano_box2.png';
import Piattaforma_box2 from '../../assets/Piattaforma_box2.png';
import Servizi_box2 from '../../assets/Servizi_box2.png';

</script>

<template>
    <div class="flex flex-col justify-center items-center">
        <h2 class="size32 colorDarkBlue mt-20 mb-40 text-center">Offriamo alle PMI supporto nei seguenti ambiti</h2>
        
        <div class="flex justify-center items-center space-x-30 mb-20">
            
            <div class="flex flex-col justify-center items-center w-60">
                <img :src="Guru_box2" alt="" class="h-55 mb-3">
                <h5 class="colorGray1 size18 my-2">Welfare Guru</h5>
                <p class="size18_2 colorGray1 text-center">per un piano di welfare aziendale personalizzato</p>
            </div>
            
            <div class="flex flex-col justify-center items-center w-60">
                <img :src="Piano_box2" alt="" class="h-55 mb-3">
                <h5 class="colorGray1 size18 my-2">Gestione del piano</h5>
                <p class="size18_2 colorGray1 text-center">welfare e dei fornitori di servizi a livello locale</p>
            </div>
                        
            <div class="flex flex-col justify-center items-center w-60">
                <img :src="Servizi_box2" alt="" class="h-55 mb-3">
                <h5 class="colorGray1 size18 my-2">Piattaforma welfare</h5>
                <p class="size18_2 colorGray1 text-center">accessibile da qualunque tipo di dispositivo</p>
            </div>

            <div class="flex flex-col justify-center items-center w-60">
                <img :src="Piattaforma_box2" alt="" class="h-55 mb-3">
                <h5 class="colorGray1 size18 my-2">Servizi welfare</h5>
                <p class="size18_2 colorGray1 text-center">in ambito flexible benefit & employee caring</p>
            </div>

        </div>
    </div>
</template>