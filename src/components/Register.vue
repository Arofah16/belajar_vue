<template>
    <div id="app">
        <!-- <p v-once>{{isAktif ? 'succes' : 'danger'}}</p> -->
        <!-- ini tidak akan lagi mengubah `foo`! -->
        <h3 v-text="message"></h3>
        <input type="text" v-model="message">
        <P>Bilangan ini adalah bilangan {{infoBIlangan}}</P>
        <p>
            <button @click="handleKlik">klik</button>
        </p>
        <!-- <button v-bind:class="{active: menu === 'home'}" @click="menu='home'">Home</button>
        <button v-bind:class="{active: menu === 'about'}" @click="menu='about'">About</button>
        <button v-bind:class="{active: menu === 'contact'}" @click="menu = 'contact'">Contact</button> -->
    <p>{{framework}}</p>
        <div>
        <label> <input type="checkbox" value="react" v-model="framework">React</label>
        <label> <input type="checkbox" value="vue js" v-model="framework">Vue js</label>
        <label> <input type="checkbox" value="Angular" v-model="framework">Angular</label>
    </div>
    
    </div>
</template>
<script>
    export default {
        data() {
            return {
                // number, string, bolean,objek
                message: "selamat datang",
                isAktif: false,
                bil: 1,
                barang1: 45000,
                barang2: 30000,
                menu: 'home',
                framework:[]
            }
        },
        methods: {
            handleKlik: function(){
                return this.bil++
            }

        },
        computed: {
            totalBayar: function () {
                return this.bil * 20000
            },
            jumlahTotal: function () {
                return this.barang1 + this.barang2
            },
            infoBIlangan: function(){
                return this.bil%2 === 0 ? 'GENAP' : 'GANJIL'
            }
        }
    }
</script>
<style scoped>
    .active{
        background-color: aquamarine;
        border: 0;
        padding: 5px;
    }

</style>