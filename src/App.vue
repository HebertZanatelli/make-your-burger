<template>
  <navbar :alt="alt_logo" :logo="end_logo"/>
  <router-view />
  <rodape />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Rodape from './components/rodape.vue';
export default {
  components: { Navbar, Rodape },
  data(){
    return{
      end_logo: "/img/logo.png",
      alt_logo: "Make Your Burguer"
    }
  }
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  font-family: Helvetica, sans-serif;
  box-sizing: border-box;
}

.main-container{
  margin: 50px;
  min-height: calc(100vh - 174px);

}

h1{
  text-align: center;
  font-size:  42px;
  margin-bottom: 30px;
  color: #222;
}
</style>
