<template>
  <div>{{message}}</div>
  <child ></child>
</template>


<script>
import Child from './components/Child.vue';

export default {
  components: {
    Child,
  },
  data() {
    return {
      message: 'Vue is working just fine!'
    }
  }
}
</script>

<style>

body {
  color: rgb(230, 46, 46);
}
</style>

