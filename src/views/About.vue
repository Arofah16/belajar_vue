<template>
  <div class="about">
    <h3> membuat direktif v-html: <span v-html="rawHtml"></span></h3>
    <!-- <button v-bind:id="dynamicId">v-bind</button> -->
    <!-- <form>
      <label for="">Nama: </label>
      <input type="text" id="name" v-model="form.nama"><br><br>
      <label for="">Email: </label>
      <input type="email" id="uname" v-model="form.username"><br><br>
      <input type="submit" value="save">
    </form> -->
    <!-- <ul>
      <li v-for="(k,index) of lessons" >{{index+1}}-{{k}}</li>
    </ul> -->
    <h3>mencari bilangan genap dengan menggunakan v-for(latihan v-for) {{numbers}}</h3>
    <ul>
      <li v-for="num in cariBilanganGenap(numbers)" :key="num">{{num}}</li>
    </ul>
  </div>
</template>
<script>
  export default {
    data(){
      return{
        lessons:['filsafat','psikologi','sosiologi'],
        numbers:[1,2,3,4,5,6,7],
      }
    },
    methods:{
      cariBilanganGenap: function(data){
        return data.filter(angka =>{
          return angka % 2 == 0
        })
      }
    }
  }

</script>