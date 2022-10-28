<template>
<HomePage></HomePage>
</template>

<script>
import HomePage from "@/components/HomePage";
export default {
  name: 'App',
  components: {
      HomePage
  }
}
</script>

<style lang="scss">
#app {
    height: 100%;
    background-color: #0A142F;

  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
