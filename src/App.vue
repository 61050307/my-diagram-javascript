<template>
  <v-app>
    <Header/>
    <Content/>
  </v-app>
</template>


<script>
import Header from "./components/Header.vue";
import Content from "./components/Content.vue"
export default {
  name : "app",
  components:{
    Header,
    Content
  }
}
</script>

<style>

</style>