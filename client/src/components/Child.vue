<template>
  <li :hover="hover" v-on:mouseover="hover = true"
        v-if="!hover">
    {{ message }}
  </li>
  <li v-else v-on:mouseleave="hover = false">Where did it go?</li>

</template>

<script>

export default {
  props: ["message"],
  data () {
    return {
      hover: false
  }}
};

</script>

<style scoped>

  li {
    width: 50%;
    height: 20px;
    background-color: rgb(157, 143, 143);
    color: rgb(143, 28, 143);
    list-style-type: circle;
  }

  li:hover {
    width: 50%;
    height: 20px;
    background-color: rgb(157, 143, 143);
    color: rgb(143, 28, 143);
    cursor: pointer;
    list-style-type: disc;
  }


</style>
