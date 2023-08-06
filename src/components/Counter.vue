<template>
    <div class="counter">
        <h1>
            <slot name="title"></slot>
        </h1>
        <p>
            <slot name="content"></slot>
        </p>
    </div>
</template>


<script setup>

</script>


<style>

.counter{
    width: 80px;
}
.counter h1{
    text-align: center;
    font-family: 'poppins-semi-bold';
}
.counter p{
    color: #BFB8B8;
    font-size: 14px;    
    text-align: center;
    font-family: 'poppins';
}

</style>