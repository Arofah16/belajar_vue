<template>
  <div class="about">
    <h1>{{data}}</h1>
    <h3> membuat direktif v-html: <span v-html="rawHtml"></span></h3>
    <button v-bind:id="dynamicId">v-bind</button>
  </div>
</template>
<script>
  export default {
    data() {
      return {
        dynamicId:true,
        data: "Semangat Arofah"
      }
    }
  }
</script>