<script setup>
import logo_bw from "../../assets/box11/logo_bw.png";
import italy_flag from "../../assets/box11/italy_flag.png";

</script>

<template>
    <div class="footer flex flex-col items-center">

        <div class="flex flex-col w-[200px] justify-center items-center text-center mt-20">
            <div class="flex justify-center items-center text-center">
                <img :src="logo_bw" alt="logo mysarma bw">
                <h5 class="size24_3 text-white">MySarma</h5>
            </div>
            <img :src="italy_flag" alt="bandiera italia" class="my-5 w-40">
            <p class="size14 colorLightGray2">Il welfare aziendale tutto italiano a portata di PMI.</p>
        </div>


        <div class="linkContainer flex-col w-full px-5">

            <div class="flex justify-between mt-10">
                <div class="flex flex-col ">
                    <h5 class="text-white size18">Chi siamo</h5>
                    <ul>
                        <li class="size18_2 colorGray2 mt-2">Vision & Mission</li>
                        <li class="size18_2 colorGray2 mt-2">Il gruppo Omninext</li>
                        <li class="size18_2 colorGray2 mt-2">Contattaci</li>
                    </ul>
                </div>
                <div class="flex flex-col w-[150px]">
                    <h5 class="text-white size18">Soluzioni welfare</h5>
                    <ul>
                        <li class="size18_2 colorGray2 mt-2">Flexible benefit</li>
                        <li class="size18_2 colorGray2 mt-2">Premio di risultato</li>
                        <li class="size18_2 colorGray2 mt-2">Performance Menagement</li>
                    </ul>
                </div>
            </div>

            <div class="flex justify-between mt-15">
                <div class="flex flex-col ">
                    <h5 class="text-white size18">Seguici su</h5>
                    <ul>
                        <li class="size18_2 colorGray2 mt-2">Linkedin</li>
                    </ul>
                </div>
                <div class="flex flex-col me-5">
                    <div class="mb-15">
                        <h5 class="size18 colorViolet1">Piano GO!</h5>
                        <h5 class="size18 colorViolet2">Piano PRO</h5>
                    </div>
                    <h5 class="size18 colorGray2">Diventa partner</h5>
                </div>
            </div>

            <div class="divider2 mt-10 mb-5"></div>

            <div class="flex flex-col">
                <p class="size14 colorGray2 mb-3">Copyright © MySarma srl - Tutti i diritti riservati</p>
                <p class="size14 colorGray2">Privacy e Cookie Policy</p>
            </div>
        </div>
    </div>
</template>



<style scoped>
.footer {
    height: 735px;
    background-color: #112340;
}

.linkContainer {
    height: 150px;
}

.divider {
    height: 150px;
    width: 0;
    border: 1px solid #89898955;
    border-radius: 50px;
}

.divider2 {
    height: 0;
    width: 100%;
    border: 1px solid #89898955;
}
</style>