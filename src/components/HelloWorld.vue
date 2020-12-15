<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <!-- <h1>{{mesage}}</h1> -->
    <p>
      For a guide and recipes on how to configure / customize this project,<br />
      check out the
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener"
        >vue-cli documentation</a
      >
    </p>
    
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
// var app = new Vue({
//   el:"#app",
//   data:{
//     message:"hallo semangat arofah"
//   }
// })
</script>

