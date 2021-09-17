<template>
  <li>
    {{ message }}
  </li>

</template>

<script>

export default {
  props: ["message"],
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
