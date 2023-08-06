<template>
    <div id="block">
        <hr>
        <div id="numbers_1">
            <div class="inside">
                <div class="fifty">50+</div>
                <p>Projects Completed</p>
            </div>
            <div class="inside">
                <div class="forty">45+</div>
                <P>GitHub Repository</P>
            </div>
        </div>
        <hr>
        <div id="numbers_2">
            <div class="inside">
                <div class="five">5+</div>
                <p>Years of expérience</p>
            </div>
            <div class="inside">
                <div class="sevenHundred">700+</div>
                <P>Youtube Suscribers</P>
            </div>
        </div>
        <hr>
    </div>
</template>


<script>

</script>


<style>

#block{
    padding: 25px;;
}
#numbers_1 p, #numbers_2 p{
    font-family: 'poppins';
    font-size: 8px;
    color: #BFB8B8;
}

#numbers_1, #numbers_2{
    height: 112px;
    display: flex;
    align-content: center;
    align-items: center;
    justify-content: space-around;
    
}

.inside{
    display: flex;
    flex-direction: column;
    align-items: center;
}

.fifty, .forty, .five, .sevenHundred{
    font-family: 'poppins-semi-bold';
    font-weight: 700;
    font-size: 26px;
}

hr {
    color: #0000002a;
}
</style>