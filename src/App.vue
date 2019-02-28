<template>
  <div class="container">
    <app-header></app-header>
    <app-list-game v-bind:myJson="myJson"></app-list-game>
  </div>
</template>

<script>

  import json from "./json/games.json";
  import Header from "./components/Header.vue";
  import ListGame from "./components/ListGame.vue";
  

export default {
  data: function(){
    return{
      myJson: json,
    }
  },
  components:{
    'app-header': Header,
    'app-list-game' : ListGame,
  }
}
</script>

<style>

</style>
