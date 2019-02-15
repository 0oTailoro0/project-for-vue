<template>
    <div>
      info
      <button @click="add()">弹出</button>
    </div>
</template>

<script>
  import store from '@/store'
  export default {
    name: 'Info',
    store,
    methods: {
      add(){
        console.log('add item')
        store.commit('increase')
      }
    }
  }
</script>

<style scoped>

</style>
