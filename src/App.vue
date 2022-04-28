    <template>
    <div id="app">
      <h1>Life cycle method in Vue Js</h1>
      <SignUp />
      <Login />
    </div>
    </template>

  <script>
  import SignUp from "./components/SignUp.vue";
import Login from "./components/Login.vue";


  export default {
    name: 'App',
    components: {
    SignUp,
    Login
}
  };
  </script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
