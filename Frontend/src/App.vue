<!-- fichier central de l'qpplication Vue.-->

<template>
    <div id="app">
      <Navi></Navi>
      <router-view></router-view>
    </div>
</template>

<script>
import Navi from "./components/Navi";

export default {
    name: "App",
    components: {
      Navi
    }
}
</script>

<style>
  body {
    background: #EB5A77;
    background: linear-gradient(90deg, #EB5A77 0%, #ec254c 100%);
  }
</style>
