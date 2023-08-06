<template>
    <a id="button" :style="{ 'backgroundColor': '#' + background }">
        {{ props.content }}
    </a>
</template>


<script setup>
import { defineProps } from 'vue';

const props = defineProps({
    content: String,
    background: String,
    color: String,
})



</script>


<style scoped>
#button{
    display: block;
    margin-top: 30px;
    margin-bottom: 12px;
    width: 131px;
    height: 32px;
    text-align: center;
    box-shadow: 0px 4px 4px 0px #00000040;
    
}

</style>