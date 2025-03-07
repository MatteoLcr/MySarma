<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel } from '@headlessui/vue'
</script>

<template>
    <div class="answare">
        <Disclosure v-slot="{ open }">
            <DisclosureButton class=" flex justify-between w-full py-2 text-left">
                <span class="size18 colorBlue1">Welfare aziendale</span>
                <svg :class="open ? 'rotate-180' : ''" class="w-5 h-5 transition-transform" viewBox="0 0 20 20"
                    fill="currentColor">
                    <path fill-rule="evenodd"
                        d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                        clip-rule="evenodd" />
                </svg>
            </DisclosureButton>
            <DisclosurePanel class="p-4 bg-white">
                <ul>
                    <li class="size18_2 colorBlue1">Cos'è il welfare </li>
                    <li class="size18_2 colorBlue1">Come posso attrarre talenti</li>
                    <li class="size18_2 colorBlue1">Storie attrattive</li>
                    <li class="size18_2 colorBlue1">Normative e vantaggi fiscali</li>
                </ul>
            </DisclosurePanel>
        </Disclosure>
    </div>
    
    <div class="answare">
        <Disclosure v-slot="{ open }">
            <DisclosureButton class=" flex justify-between w-full py-2 text-left">
                <span class="size18 colorBlue1">Chi siamo</span>
                <svg :class="open ? 'rotate-180' : ''" class="w-5 h-5 transition-transform" viewBox="0 0 20 20"
                    fill="currentColor">
                    <path fill-rule="evenodd"
                        d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                        clip-rule="evenodd" />
                </svg>
            </DisclosureButton>
            <DisclosurePanel class="p-4 bg-white">
                <!-- EVENTUALE TESTO O LINK -->
            </DisclosurePanel>
        </Disclosure>
    </div>
    
    <div class="answare">
        <Disclosure v-slot="{ open }">
            <DisclosureButton class=" flex justify-between w-full py-2 text-left">
                <span class="size18 colorBlue1">Soluzioni welfare</span>
                <svg :class="open ? 'rotate-180' : ''" class="w-5 h-5 transition-transform" viewBox="0 0 20 20"
                    fill="currentColor">
                    <path fill-rule="evenodd"
                        d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                        clip-rule="evenodd" />
                </svg>
            </DisclosureButton>
            <DisclosurePanel class="p-4 bg-white">
                <!-- EVENTUALE TESTO O LINK -->
            </DisclosurePanel>
        </Disclosure>
    </div>
    
    <div class="answare">
        <Disclosure v-slot="{ open }">
            <DisclosureButton class=" flex justify-between w-full py-2 text-left">
                <span class="size18 colorBlue1">Blog</span>
                <svg :class="open ? 'rotate-180' : ''" class="w-5 h-5 transition-transform" viewBox="0 0 20 20"
                    fill="currentColor">
                    <path fill-rule="evenodd"
                        d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                        clip-rule="evenodd" />
                </svg>
            </DisclosureButton>
            <DisclosurePanel class="p-4 bg-white">
                <!-- EVENTUALE TESTO O LINK -->
            </DisclosurePanel>
        </Disclosure>
    </div>
</template>

<style scoped>
.answare {
    border-bottom: 1px solid #e9e9e9;   
}
</style>