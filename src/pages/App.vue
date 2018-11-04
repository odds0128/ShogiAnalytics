<template>
  <div id="app">
    <my-header id="header"/>
    <div id="body">
      <img src="@/assets/japanese-chess/piece/60x64/sOu.png">
      <inputForm/>
    </div>
  </div>
</template>

<script>
import myHeader from "../components/myHeader.vue";
import inputForm from "../components/inputForm"

window.onload = function(){
  const header_height = document.getElementById('header').clientHeight;
  const css_body = document.getElementById('body')
  css_body.style.marginTop = header_height + 20 + 'px';
};

export default {
  name: "App",
  components: {
    myHeader,
    inputForm
  }
};
</script>

<style>
#body {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
