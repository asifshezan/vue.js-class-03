<template>
    <div>
        <p v-if="error.length">
            <b>Please conplete your errors</b>
            <ul>
                <li v-for="e in error" v-bind:key="e.name">
                    {{ e }}
                </li>
            </ul>
        </p>
        <form @submit="login">
            <input type="text" placeholder="enter name" v-model="name"><br><br>
            <input type="password" v-model="password"/><br><br>
            <button type="submit">Login</button>
        </form>
    </div>
</template>
<script>
export default {
    name: 'AsifLoginvalidation',

    data() {
        return {
            error:[],
            name:null,
            password:null
        };
    },

    mounted() {
        
    },

    methods: {
        login(e){
            this.error=[];
            if(this.name & this.password){
                console.warn('no error');
            }
            if(!this.name){
                this.error.push('user name is required');
            }
            if(!this.password){
                this.error.push('password is required');
            }
            console.log("Hello",this.error);
            e.preventDefault();
            
        }
    },
};
</script>