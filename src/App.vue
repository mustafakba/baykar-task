<template>
<HomePage></HomePage>
<DigitalAgency></DigitalAgency>
<OurSolutions></OurSolutions>
<ServicePage></ServicePage>
<LatestProjects></LatestProjects>
<HappyClients></HappyClients>
    <BlogFrom></BlogFrom>
<CategoriesPage></CategoriesPage>
    <FooterComponent></FooterComponent>
</template>

<script>
import HomePage from "@/components/HomePage";
import DigitalAgency from "@/components/DigitalAgency";
import OurSolutions from "@/components/OurSolutions";
import ServicePage from "@/components/ServicePage";
import LatestProjects from "@/components/LatestProjects";
import HappyClients from "@/components/HappyClients";
import BlogFrom from "@/components/BlogFrom";
import CategoriesPage from "@/components/CategoriesPage";
import FooterComponent from "@/components/FooterComponent";
export default {
  name: 'App',
  components: {
      FooterComponent,
      CategoriesPage,
      BlogFrom,
      HappyClients,
      LatestProjects,
      ServicePage,
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
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
