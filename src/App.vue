<template>
  <div class="app">
    <p>{{ name }} - {{ age }}</p>
    <button @click="changeNameAndAge('this shit is amazing', 69)">
      change name & age
    </button>
  </div>
</template>
<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  components: {},
  data() {
    return {
      name: "SUP BRO",
      age: 25 as number | string,
    };
  },
  methods: {
    changeNameAndAge(name: string, age: number | string) {
      this.name = name;
      this.age = age;
    },
  },
})
export default class App extends Vue {
  name: any;
  changeNameAndAge: any;
  age: any;
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
  height: 100vh;
  background: #2c3e50;
  display: grid;
  place-items: center;
}
</style>
