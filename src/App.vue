<template>
<HomePage></HomePage>
<DigitalAgency></DigitalAgency>
<OurSolutions></OurSolutions>
</template>

<script>
import HomePage from "@/components/HomePage";
import DigitalAgency from "@/components/DigitalAgency";
import OurSolutions from "@/components/OurSolutions";
export default {
  name: 'App',
  components: {
      HomePage,
      DigitalAgency,
      OurSolutions
  }
}
</script>

<style lang="scss">
#app {
    height: 100%;
    background-color: #0A142F;
    padding-bottom: 300px;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
