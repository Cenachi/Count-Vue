<template>
  <div id="container">
    <button class="button" @click="increment">Count is: {{ count }}</button>

    <button class="button" @click="reset">Reset</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
    };
  },

  methods: {
    increment() {
      this.count++;
    },

    reset() {
      this.count = 0;
    },
  },
};
</script>

<style>
#container {
  display: flex;
  justify-content: center;
}

.button {
  background-color: rgb(0, 255, 213);
  font-size: 25px;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
}
</style>
