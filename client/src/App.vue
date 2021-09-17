<template>
  <ul v-for="message in messages" :key="message">
    <child :message="message" ></child>
  </ul>

</template>


<script>
import Child from './components/Child.vue';

export default {
  components: {
    Child,
  },
  data() {
    return {
      messages: [
        'This is the first of many messages',
        'This is the second of many messages',
        'This is the third of many messages',
        'This is the fourth of many messages',
        'This is the fifth of many messages',
        'This is the sixth of many messages',
        'This is the seventh of many messages',
        'This is the eighth of many messages',
        'This is the ninth of many messages',
        'This is the last of the messages',
      ]
    }
  }
}
</script>

<style>

body {
  color: rgb(230, 46, 46);
}
</style>

