<template>
    <div>
        <input type="text" name="username" placeholder="enter your name" v-model="loginForm.username" /><br><br>
        <input type="password" name="password" placeholder="enter your password" v-model="loginForm.password" /><br><br>
        <button v-on:click="loginData">LogIn</button>
    </div>
</template>
<script>
export default {
    name: 'AsifLogin',

    data() {
        return {
            loginForm:{
                username:null,
                password:null
            }
        };
    },

    mounted() {
        
    },

    methods: {
        loginData(){
            console.log("loginData",this.loginForm)
            // console.log("lognData",this.loginForm.username,this.logForm.password)
        }
    },
};
</script>