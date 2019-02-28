<template>
    <div class="container">
        <div class="row">
            <form class="form-inline mt-3 pl-3">
                <input class="form-control" type="text" placeholder="Search Game" aria-label="Search" v-model="search">
            </form>
        </div>
        <div class="row">
            <div class="col-md-4 col-lg-3 d-flex align-items-stretch" v-for="data in filtred.slice(0, gamesToShow)" :key="data.id">
                <div class="card mt-3">
                    <div class="card-body">
                        <h5 class="card-title">{{data.name}}</h5>
                        <h6 class="card-subtitle mb-2 text-muted">Author: {{data.vendor}}</h6>
                        <p class="card-text">
                            {{data.description}}
                        </p>
                    </div>
                </div>
            </div>
        </div>
         <button type="button" class="btn btn-secondary btn-lg mt-3" @click="gamesToShow +=9">More Games</button>
    </div>   
</template>

<script>

import json from '../json/games.json';

export default {
    props:['myJson'],
    data:function(){
        return{
            search:'',
            gamesToShow: 8
        }
    },
    computed:{
      filtred: function(){
          return this.myJson.filter(data =>
            data.name.match(new RegExp(this.search, 'i')))
      }
  }
}
</script>

<style>

</style>
