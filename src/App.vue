<template>
  <AppHeader
    v-bind:appTitle="message"
    v-on:change="changeMessage"
  />
  <div></div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'

export default {
  name: 'App',
  components: {
      AppHeader
  },
  data(){
    return {
      message: '앱 헤더 컴포넌트'
    }
  },
  methods: {
    changeMessage(){
      this.message = '변경됨'
    }
  }
}
</script>

<style>
</style>
