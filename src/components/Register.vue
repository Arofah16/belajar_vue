<template>
    <div id="app">
        <p>{{message }}</p>
        <!-- ini tidak akan lagi mengubah `foo`! -->
        <button>Change it</button>
    </div>
</template>
<script>
export default{
    data(){
        return{
            message:"selamat datang "
        }
    }
}
</script>