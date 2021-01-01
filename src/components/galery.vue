<template>
    <div>
        <!-- <h2>membuat form input binding</h2>
    <input v-model="pesan" placeholder="isikan disini">
    <p>isi pesanya adalah : {{pesan}}</p> -->

    <!-- <span>membuat pesan multiline</span>
    <p style="white-space: pre-line;">{{pesan}}</p>
    <textarea v-model="pesan" placeholder="tambahkan kata- kata dibawah"></textarea> -->

    <h2>membuat checkbox dengan v-model</h2>
    <!-- <input type="checkbox" id="checkbox" v-model="checked">
    <label for="checkbox">{{checked}}</label> -->
    <input type="checkbox" id="html" value="HTML" v-model="checked">
    <label for="html">HTML</label>
    <input type="checkbox" id="html" value="CSS" v-model="checked">
    <label for="html">CSS</label>
    <br>
    <span>kelas yang dicentang:{{checked}}</span>

    <H2>Membuat Radio button</H2>
    <input type="radio" id="laki-laki" value="laki-laki" v-model="picked">
    <label for="laki-laki" >laki-laki</label>
    <input type="radio" id="perempuan" value="perempuan" v-model="picked">
    <label for="permepuan">perempuan</label>
    <br>
    <span>jenis kelamin : {{picked}}</span>

    <h2>membuat pilihan selected</h2>
    <select v-model="selected">
        <option value="">masukkan pilihan anda:</option>
        <option>front end</option>
        <option>back end</option>
        <option>fullstack</option>
    </select>
    <span>pilihanku adalah:{{selected}}</span>
    <br>
    <h2>contoh penggunaan vue instance
{{tanggal}}
    </h2>
    <button v-on:click="count++">Anda mengklik saya {{ count }} kali.</button>
</div>
</template>
<script>
    export default{
        data(){
            return{
            pesan:"",
            checked:[],
            picked:'',
            selected:'',
            count:'' 
            }
        },
        props:['tanggal']
    }
</script>