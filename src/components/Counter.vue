<template>
  <div class="app">
    Counter is {{ $store.state.count }}
    <button @click="increment">+5</button>
    <button @click="decrement">-3</button>
  </div>

</template>

<script>
  import {  mapActions } from 'vuex'
  export default {
//    computed: mapGetters([
//
//    ]),
    methods: mapActions([
        'increment',
        'decrement'
    ])
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>
