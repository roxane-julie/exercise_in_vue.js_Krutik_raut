<template>
    <div id="hello">
        <h1>Hello,<br/> I am <span class="name">Roxane Breton</span></h1>
        <p class="work">Developpeur web/mobile</p>
    </div>
</template>

<script setup>
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
    padding-bottom: 200px;
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
   
    
}
</style>