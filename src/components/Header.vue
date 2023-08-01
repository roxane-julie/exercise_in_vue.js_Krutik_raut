<template>
    <div id="header">

        <div class="logo">        
            <img src="../assets/reboot13_.png" alt="">
            
        </div>

        <div class="burger" @click="state=!state" :class="{'burger--open':state}">
            <div class="trait"></div>
            <div class="trait"></div>
            <div class="trait"></div>
            
        </div>
   

    <div class="menu--burger" :class="{'open':state}">

    </div> 
    </div>
</template>

<script setup>
import { ref } from 'vue';

const state= ref(false);

</script>

<style scoped>
#header{
    display: flex;
    align-items: center;
    justify-content: space-between;
    
}
#header .burger .trait{
    height: 3px;
    width: 23px;
    background: #000;
    margin-bottom: 3px;
}
#header .menu--burger{
    height: 100vh;
    width: 100%;
    background: #000;
    position: fixed;
    top: 0;
    left: 100%;
    transition: 0.3s;
}
#header .open{
    left: 0%
}
.burger--open{
    z-index: 2;
    background: white;
}
</style>