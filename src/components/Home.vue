<template>
    <div>
        <p v-html="rowHtml"></p>
        <h1 class="homestyle">Class and Style Component</h1>
        <h1 v-bind:style="{color:colorKey}">Style Component</h1>
        <h1 v-bind:style="{color:'blue'}">Style Component</h1>
        <h1 v-bind:class="{display:show}">Class Bindings with object</h1>
        <h1 v-bind:class="[aclass]">Class Bindings with Array</h1>
        <h1 v-bind:class="[show?'yesShow':'noShow']">Class Bindings with Array</h1>
    </div>
</template>
<script>
// import Products from './Products.vue';
// import Users from './Users.vue'


export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name:'Home',
    data(){
        return {   
            rowHtml:"<h1>Home Component</h1>", 
            show:true,
            aclass:'array',
            colorKey:'red'
        }
    },
};
</script>

<style scoped>
    .homestyle{
        background-color:rgb(218, 137, 232);

    }
    .display{
        background-color: burlywood;
    }
    .array{
        background-color: cyan;
    }
</style>