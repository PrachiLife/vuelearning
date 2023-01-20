<template>
  <div class="">
    <input type="text" v-model="data" />
    <div v-on:click="getData()">{{ data }} Testing</div>
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
    getData() {
      console.log("hello");
    },
  },
};
</script>

<style></style>
