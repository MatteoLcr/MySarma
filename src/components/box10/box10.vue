<script setup>
import letter from '../../assets/box10/letter.png';
</script>

<template>
    <div class="flex flex-col lg:flex-row justify-evenly items-start lg:items-center lg:h-[400px] mt-40 lg:mt-60 px-5 lg:px-0" :style="{
        backgroundImage: `url(${letter})`,
        backgroundColor: '#426BD1',
        backgroundBlendMode: 'multiply',
    }">
        <div class="flex flex-col justify-center items-start my-20 lg:mt-0 lg:mt-0">
            <h5 class="size32 text-white mb-5 lg:mb-0">Resta aggiornato</h5>
            <p class="size18_2 colorLightGray2">Iscriviti alla newsletter per ricevere aggiornamenti </p>
            <p class="size18_2 colorLightGray2">sulle nuove offerte e partener MySarma</p>
        </div>
        <form class="flex flex-col justify-end items-end lg:flex-row lg:justify-center lg:items-center ">
            <div>
                <label for="email" class="block size18 colorLightGray2">Il tuo indirizzo mail</label>
                <input id="email" type="email" v-model="email" placeholder="@"
                    class=" p-2 mt-1 bg-white border rounded-md w-[400px] h-[50px]" />
            </div>

            <button type="submit" class="btnInvia ms-10 mt-8">
                Invia
            </button>
            <div class="btnInviaUnder hidden lg:block ms-10 mt-8"></div>
            <div class="btnInviaUnder2 clock md:hidden ms-10 mt-8"></div>
        </form>
    </div>
</template>

<style scoped>
.btnInvia {
    height: 50px;
    width: 110px;
    border: 2px solid #112340;
    border-radius: 10px;
    color: #112340;
    z-index: 3;
}

.btnInviaUnder {
    height: 50px;
    width: 110px;
    position: relative;
    top: 5px;
    right: 145px;
    background-color: rgb(255, 255, 255);
    border-radius: 10px;
    z-index: 2;
}
.btnInviaUnder2 {
    height: 50px;
    width: 110px;
    position: relative;
    bottom: 76px;
    right: -5px;
    background-color: rgb(255, 255, 255);
    border-radius: 10px;
    z-index: 2;
}


</style>