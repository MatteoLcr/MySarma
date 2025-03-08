<script setup>
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';
import 'vue3-carousel/dist/carousel.css';

import Guru_img from '../../assets/box3/Guru_img.png';
import Pianoforte from '../../assets/box3/Pianoforte.png';
import Servizi from '../../assets/box3/Servizi.png';
import Piattaforma from '../../assets/box3/Piattaforma.png';
</script>

<template>
    <Carousel :items-to-show="1" :wrap-around="true" :space="30" class="customCarousel">
        <Slide class="slide">
            <div class="slide-content flex justify-evenly items-center rounded-3xl px-5 py-6"
                style="background-color: #283B6C; width: 95%;">
                <div class="text-content flex flex-col justify-start items-start">
                    <h3 class="text-white size72 w-100">Welfare Guru</h3>
                    <p class="text-white size18_2 w-150">
                        È un professionista capace di affiancare le aziende in tutte le fasi
                        proprie all'attivazione di un piano welfare. Sia tu abbia già un sistema
                        premiale basato su premi di risultato o incentivi diversi, sia che per te
                        sia la prima esperienza, il Welfare Guru saprà consigliarti la migliore
                        soluzione.
                    </p>
                    <button class="text-white mt-20 mb-5">Scopri di più</button>
                </div>
                <img :src="Guru_img" alt="Welfare Guru" style="scale: 1.5;" />
            </div>
        </Slide>

        <Slide class="slide">
            <div class="slide-content flex justify-evenly items-center rounded-3xl px-15"
                style="background-color: #716ACA; width: 95%;">
                <div class="text-content flex flex-col justify-start items-start">
                    <h3 class="text-white size72 w-100">Gestione del piano</h3>
                    <p class="text-white size18_2 w-150">
                        L progettare Piani di Welfare on top, realizzando un’analisi delle caratteristiche delle
                        popolazione aziendale e dei fabbisogni dei dipendenti. Siamo in grado di fornire consulenza
                        specializzate nella costruzione delle categorie omogene e nell’implementazione di un rete di
                        servizi disegnata su misura delle esigenze dei clienti.
                    </p>
                    <button class="text-white mt-20 mb-5">Scopri di più</button>
                </div>
                <img :src="Pianoforte" alt="Pianista" style="scale: 0.8;" />
            </div>
        </Slide>

        <Slide class="slide">
            <div class="slide-content flex justify-start items-center rounded-3xl px-15 position-relative"
                style="background-color: #426BD1; width: 95%;">
                <div class="text-content flex flex-col justify-start items-start">
                    <h3 class="text-white size72 w-200">Soluzioni welfare </h3>
                    <h3 class="text-white size72 w-200">esclusive </h3>
                    <p class="text-white size18_2 w-150">
                        Libertà di scelta dei fornitori Ampia gamma di fornitori già presenti in piattaforma e
                        possibilità di aggiungere fornitori di fiducia presso cui spendere il proprio credito welfare.
                        Nessun costo fisso per l’attivazione e nessun problema finanziario poiché non è necessario
                        versare interamente e in anticipo tutto l’importo del credito welfare. Servizio di assistenza
                        telefonica dedicata per il referente aziendale e servizio di customer care via chat ed email per
                        i dipendenti.
                    </p>
                    <button class="text-white mt-10 mb-8">Scopri di più</button>
                </div>
                <img :src="Servizi" alt="Servizi" style="position: absolute; right: 0px;" />
            </div>
        </Slide>

        <Slide class="slide">
            <div class="slide-content flex justify-start items-center rounded-3xl px-15 py-3"
                style="background-color: #299882; width: 95%;">
                <div class="text-content flex flex-col justify-start items-start">
                    <h3 class="text-white size72 w-100">Piattaforma </h3>
                    <h3 class="text-white size72 w-200">web dedicata </h3>
                    <p class="text-white size18_2 w-150">
                        Sulla nostra piattaforma dedicata potrai gestire in autonomia il tuo piano di benefit aziendale
                        utilizzando qualsiasi gingillo di cui disponi (smartphone, tablet o computer). La piattaforma
                        MySarmaNet è disponibile tramite connessione internet e supporta il tuo team nella gestione
                        operativa.
                    </p>
                    <button class="text-white mt-20 mb-5">Scopri di più</button>
                </div>
                <img :src="Piattaforma" alt="Piattaforma" style="position: absolute; right: 0px; bottom: 50px; scale: 0.9;" />
            </div>
        </Slide>

   
        <template #addons>
            <!-- <Navigation /> -->
            <Pagination/>
        </template>

    </Carousel>
</template>

<style scoped>

.customCarousel {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 40px 0;
}


.carousel__pagination {
    margin-top: 10px;
}

.carousel__pagination-button {
    background-color: gray;
    opacity: 0.7;
}

.carousel__pagination-button--active {
    background-color: white;
}

</style>
