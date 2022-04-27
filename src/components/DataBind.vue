<template>
    <div>
        <h1>{{ message }}</h1>
        <h2 style="white-space:pre-line;">{{ message }}</h2>
        <input type="text" v-model="message" name="" value="">
        <textarea style="padding:10px; margin-left:10px;" rows="" type="text" v-model="message" cols=""></textarea>
    </div>
</template>
<script>
export default {
    name: 'AsifDatabind',

    data() {
        return {
            message:'Hello'
        };
    },

    mounted() {
        
    },

    methods: {
        
    },
};
</script>