    <template>
    <div id="app">
      <h1>Send Props child to parent in Vue Js</h1>
      <h2>{{ title }}</h2>
      <Child v-on:changeTitle="updateTitle($event)" />
    </div>
    </template>

  <script>
  import Child from "./components/child.vue";

  export default {
    name: 'App',
    components: {
    Child,
    },data(){
    return {
      title:"props tutorial"
    }
  },methods:{
    updateTitle(title){
      this.title=title
    }
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
