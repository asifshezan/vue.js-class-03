<template>
    <div>
        <input type="text" v-model="signup.username" placeholder="enter your name"><br><br>
        <input type="password" v-model="signup.password" placeholder="enter your password"><br><br>
        <p>Choose Hobbies</p>
        <input type="checkbox" id="cricket" value="cricket" v-model="signup.hobbies" />
        <label for="cricket">Cricket</label>
        <input type="checkbox" id="football" value="football" v-model="signup.hobbies" />
        <label for="football">Football</label>
        <p>Select Gender</p>
        <input type="radio" id="male" value="male" v-model="signup.gender" />
        <label for="male">Male</label>
        <input type="radio" id="female" value="female" v-model="signup.gender" />
        <label for="female">Female</label><br><br><br>
        <button v-on:click="signupuser">Sign Up</button><br><br><br><br>
    </div>
</template>
<script>
export default { 
    name: 'AsifSignup',

    data() {
        return {
            signup:{
                username:null,
                password:null,
                hobbies:[],
                gender:null
            }
        };
    },

    mounted() {
        
    },

    methods: {
        signupuser(){
            console.warn(this.signup)
        }
    },
};
</script>