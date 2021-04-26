<template>
  <div>
    <h1>{{ name }}</h1>
  </div>
</template>

<script>
export default {
  name: "Home3",
  data() {
    return {
      name: "Home Component",
    };
  },

  beforeDestroy() {
    alert("hello");
    console.warn("before destroy"); //called before destroyed
  },

  destroyed() {
    alert("destroyed");
    console.warn("destroyed"); //after destroyed
  }
};
</script>