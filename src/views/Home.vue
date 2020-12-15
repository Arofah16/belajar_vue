<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld message="Welcome to Your Vue.js App" />
    <REG />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import REG from "@/components/Register.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
    REG,
  }
};
</script>
