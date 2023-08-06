<template>
    <div id="hello">
        <h1>Hello,<br/> I am <span class="name">Roxane Breton</span></h1>
        <p class="work">Developpeur web/mobile</p>

        <Button content="Contact" background="ffffff" color="000000"/>
        <Button content="About" background="5E3AEE" color="ffffff"/>

        <Laptop/>
</div>
        <InfoCounter/>

        <AbitAboutMe/>

    
</template>

<script setup>
import Button from './Button.vue'
import Laptop from './Laptop.vue'
import AbitAboutMe from './aBitAbout.vue'
import InfoCounter from './InfosCounter.vue'
</script>

<style>

/* #hello {
    
} */
#hello {
    display: flex;
    justify-content: space-between;
    flex-direction: column;
    font-family: 'poppins';
    background: #F0F0F3;
    margin:20px;
    align-items: center;
    padding-top: 20px;
    
    }
#hello h1{
    text-align: center;
    font-weight: 700;    
    font-family: 'poppins-semi-bold';
    margin: 0;
    
}

#hello .name {
    color: #5E3AEE;
}
#hello .work {
    color: #696969;
    margin: 0;
    font-size: 14px;
   
    
}
</style>