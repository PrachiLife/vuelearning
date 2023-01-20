<template>
  <div class="">
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
};
</script>

<style></style>
