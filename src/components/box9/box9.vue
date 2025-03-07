<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel } from '@headlessui/vue'
</script>

<template>

    <div class="flex flex-col justify-center items-center mt-25 mb-8 lg:mt-50 lg:mb-20">
        <h5 class="size24_2 lg:size32 colorBlue2">Domande frequenti</h5>
    </div>

    <div class="lg:w-[800px] mx-auto space-y-2">
        <!-- Primo elemento -->
        <div class="answare">
            <Disclosure v-slot="{ open }">
                <DisclosureButton class=" flex justify-between w-full px-4 py-2 text-left">
                    <span class="size18_3 colornightBlue">Che differenza c’è tra il Piano Go e il Piano Pro?</span>
                    <svg :class="open ? 'rotate-180' : ''" class="w-5 h-5 transition-transform" viewBox="0 0 20 20"
                        fill="currentColor">
                        <path fill-rule="evenodd"
                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                            clip-rule="evenodd" />
                    </svg>
                </DisclosureButton>
                <DisclosurePanel class="p-4 size18_2 colorGray2 bg-white">
                    Il Piano Go è stato pensato che gestire il welfare aziendale derivante da CCNL o i fringe benefits.
                    Per
                    godere della fiscalità agevolata è necessario rispettare nell’erogazione di questi beni il limite
                    massimo annuo di 258, 23 euro previsto dal Tuir per ciascun dipendente. Restando entro questa
                    soglia,
                    infatti, la somma non concorre a formare reddito da lavoro dipendente. Il Piano PRO invece è non ha
                    limiti di importo e consente di accedere a tutti i servizi welfare (flexible benefits).
                </DisclosurePanel>
            </Disclosure>
        </div>

        <!-- Secondo elemento -->
        <div class="answare">
            <Disclosure v-slot="{ open }">
                <DisclosureButton class="flex justify-between w-full px-4 py-2 text-left">
                    <span class="size18_3 colornightBlue">Che servizi comprende il Piano Go?</span>
                    <svg :class="open ? 'rotate-180' : ''" class="w-5 h-5 transition-transform" viewBox="0 0 20 20"
                        fill="currentColor">
                        <path fill-rule="evenodd"
                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                            clip-rule="evenodd" />
                    </svg>
                </DisclosureButton>
                <DisclosurePanel class="p-4 size18_2 colorGray2 bg-white ">
                    Il Piano Go consente di accedere a tutti i buoni spesa, buoni carburante, buoni regalo ed alcuni
                    voucher
                    selezionati da MySarma come le esperienze o pacchetti vacanze.
                </DisclosurePanel>
            </Disclosure>
        </div>

        <!-- Terzo elemento -->
        <div class="answare">
            <Disclosure v-slot="{ open }">
                <DisclosureButton class="flex justify-between w-full px-4 py-2 text-left">
                    <span class="size18_3 colornightBlue">Come avviene la gestione del Piano Go?</span>
                    <svg :class="open ? 'rotate-180' : ''" class="w-5 h-5 transition-transform" viewBox="0 0 20 20"
                        fill="currentColor">
                        <path fill-rule="evenodd"
                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                            clip-rule="evenodd" />
                    </svg>
                </DisclosureButton>
                <DisclosurePanel class="p-4 size18_2 colorGray2 bg-white ">
                    La gestione del Piano Go è totalmente automatizzata: è possibile sottoscrivere il contratto
                    direttamente
                    online, effettuare il pagamento ed indicare beneficiari ed importi del bonus (fino a 258 euro).
                    Questi
                    riceveranno direttamente via email le credenziali per accedere alla piattaforma, mentre l’azienda
                    riceverà in automatico la fattura elettronica utile per la deduzione integrale del costo.
                </DisclosurePanel>
            </Disclosure>
        </div>

        <!-- querto elemento -->
        <div class="answare">
            <Disclosure v-slot="{ open }">
                <DisclosureButton class="flex justify-between w-full px-4 py-2 text-left">
                    <span class="size18_3 colornightBlue">Il Piano Pro comprende i servizi del Piano Go?</span>
                    <svg :class="open ? 'rotate-180' : ''" class="w-5 h-5 transition-transform" viewBox="0 0 20 20"
                        fill="currentColor">
                        <path fill-rule="evenodd"
                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                            clip-rule="evenodd" />
                    </svg>
                </DisclosureButton>
                <DisclosurePanel class="p-4 size18_2 colorGray2 bg-white ">
                    Sì, in automatico il Piano Pro comprende anche i fringe benefit previsti dal Piano Go a meno che
                    l’azienda decida di escluderlo per alcuni o tutti i dipendenti perché già erogati sotto altre forme.
                </DisclosurePanel>
            </Disclosure>
        </div>

        <!-- quinto elemento -->
        <div class="answare">
            <Disclosure v-slot="{ open }">
                <DisclosureButton class="flex justify-between w-full px-4 py-2 text-left">
                    <span class="size18_3 colornightBlue">Che servizi comprende il Piano Pro?</span>
                    <svg :class="open ? 'rotate-180' : ''" class="w-5 h-5 transition-transform" viewBox="0 0 20 20"
                        fill="currentColor">
                        <path fill-rule="evenodd"
                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                            clip-rule="evenodd" />
                    </svg>
                </DisclosureButton>
                <DisclosurePanel class="p-4 size18_2 colorGray2 bg-white ">
                    Il Piano Pro prevede tutti i servizi dei flexible benefits organizzati nelle 3 macro categorie:
                    · Versamenti: Previdenza complementare e sanità integrativa
                    · Rimborsi: Spese scolastiche, spese per non autosufficienza, trasporto pubblico locale, Interessi
                    passivi del mutuo
                    · Voucher: Viaggi, salute, benessere, cultura, sport, fringe benefits, ecc.
                </DisclosurePanel>
            </Disclosure>
        </div>

        <!-- sesto elemento -->
        <div class="answare">
            <Disclosure v-slot="{ open }">
                <DisclosureButton class="flex justify-between w-full px-4 py-2 text-left">
                    <span class="size18_3 colornightBlue">È possibile passare dal Piano Go al Piano Pro</span>
                    <svg :class="open ? 'rotate-180' : ''" class="w-5 h-5 transition-transform" viewBox="0 0 20 20"
                    fill="currentColor">
                    <path fill-rule="evenodd"
                    d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                    clip-rule="evenodd" />
                </svg>
            </DisclosureButton>
            <DisclosurePanel class="p-4 size18_2 colorGray2 bg-white ">
                Trattandosi di due fattispecie diverse non è possibile passare in automatico dal Piano Go al Piano Pro
                ma occorre sottoscrivere un nuovo contratto
            </DisclosurePanel>
        </Disclosure>
    </div>
</div>


</template>

<style scoped>
.answare {
    border-bottom: 1px solid #e9e9e9;
    padding: 25px;
}
</style>