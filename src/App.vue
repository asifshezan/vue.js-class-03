    <template>
    <div id="app">
      <h1>Props in Vue Js</h1>
      <Child v-bind:users="users" />
    </div>
    </template>

  <script>
import Child from "./components/child.vue";

  export default {
    name: 'App',
    components: {
    Child
  },data(){
    return {users:[
      {name:"asif", email:"asdif@gamil.com"},
      {name:"asif", email:"asdif@gamil.com"},
      {name:"asif", email:"asdif@gamil.com"},
      {name:"asif", email:"asdif@gamil.com"}
    ]}
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
