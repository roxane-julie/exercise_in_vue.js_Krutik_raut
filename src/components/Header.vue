<template>
    <div id="header">

        <div class="logo">        
            <img src="../assets/reboot13_.png" alt="">
            
        </div>
        <!-- MENU MOBILE-->

        <div class="burger" @click="state=!state" :class="{'burger--open':state}">
            <div class="trait"></div>
            <div class="trait"></div>
            <div class="trait"></div>
            
        </div>
   

    <div class="menu--burger" :class="{'open':state}">

    </div> 

     <!-- MENU MOBILE-->

     <!-- MENU DESKTOP-->
     <ul class="links">
        <li v-for="(link, i) in links" :key="i">{{ link.name }}</li>
     </ul>
     <!-- MENU DESKTOP-->

    </div>
</template>

<script setup>
import { ref } from 'vue';

const state= ref(false);

const links = ref([
    {name: 'Home'},
     {name: 'Project'},
     {name: 'About'},
     {name: 'Contacts'}
])

</script>

<style scoped>
#header{
    font-family: 'poppins';
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

#header .links {
    display: none;

}
@media screen and (min-width: 780px){
    #header .burger,#header .menu--burger{
        display: none;
    }
    #header .links {
    display: flex;   
    }
    #header .links li {
    list-style-type: none;
    margin-right: 20px;
    font-family: 'poppins';
    font-weight: 500;
    }


}

</style>