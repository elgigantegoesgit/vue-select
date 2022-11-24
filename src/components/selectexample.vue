<template>
  <div class="hello">
    <v-select :options="options" v-model="mydata"></v-select>
    <h1>{{ msg }}</h1>
    <p @click="mymeth">vue-selct example...</p>

    <h3>Teststring: {{ mydata }}</h3>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      options: ["foo", "bar", "baz"],
      mydata: "teststring"
    };
  },
  watch: {
    mydata(val, oldVal) {
      alert("new: ${val}, old: ${oldVal}"); // mind ${var}: see template literals!
      console.log(val + oldVal);
    }
  },
  props: {
    msg: String
  },
  methods: {
    mymeth() {
      alert("jo");
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
