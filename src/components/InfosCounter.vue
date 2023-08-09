<template>
    <div id="info--counter">
        <div class="wrapper" v-for="(counter, index) in data" :key="index">
            <div class="separator"></div>

            <div class="container--counter">
                <Counter>
                    <template #title>{{ counter[0].title }} +</template>
                    <template #content>{{ counter[0].content }}</template>
                </Counter>
                <Counter>
                    <template #title>{{ counter[1].title }} +</template>
                    <template #content>{{ counter[1].content }}</template>
                </Counter>
            </div>
            <div  v-if="index === data.length -1" class="separator"></div>
        </div>

    </div>

</template>


<script setup>
import Counter from './Counter.vue'
import { ref } from 'vue'

const data = ref([[
    {
        title: "50",
        content: "Projects completed"
    },
    {
        title: "45",
        content: "Github repository",
    }],
    [{
        title: "5",
        content: "Expérience",
    },
    {
        title: "700",
        content: "Youtube subscribers",
    }],
    
])
</script>


<style>
#info--counter{
    margin-top: 20px;
}
#info--counter .wrapper{

    padding: 0px 50px;
}
#info--counter .wrapper .container--counter{
    display: flex;
    align-items: center;
    justify-content: space-between;

}

#info--counter .separator{
    height: 5px;
    background: #F0F0F5;
    margin: 13px 0px;
}


</style>