<template>
  <div class="">
    <h1></h1>
    <input type="text" v-model="data" />
    <br /><br />
    <button v-on:click="clearData">Clear</button>
    <button v-on:click="capsData">CapsData</button>
  </div>
</template>

<script>
export default {
  name: "TestComponent",
  data: () => {
    return {
      data: null,
      d: new Date(),
    };
  },
  methods: {
    clearData() {
      this.data = null;
    },
    capsData() {
      this.data = this.data.toUpperCase();
    },
  },
  created() {
    console.log("created");
    console.log(this.d);
  },
  mounted() {
    console.log("mounted");
    console.log(this.d);
  },
  updated() {
    console.log("updated");
    console.log(this.d);
  },
};
</script>

<style></style>
