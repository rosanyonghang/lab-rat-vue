<template>
    <nav>
        <div class="logo">Logo</div>
        <div class="nav-items">
            <router-link  to='/' class="nav-item">Home</router-link>
            <router-link to='/about' class="nav-item">About</router-link>
            <div class="nav-item">Services</div>
            <div class="nav-item">Products</div>
            <div class="nav-item">Contacts</div>
        </div>
    </nav>
</template>
<script>
    export default {
        name:'Nav'
    }
</script>
<style lang="scss" scoped>
    nav{
        background:coral;
        padding:0 5vw;
        box-sizing: border-box;
        display:flex;
        height:8vh;
        width:100%;
        align-items:center;
        justify-content: space-between;
        .nav-items{
            display: flex;
            justify-content: space-between;
            width:30%;
        }
    }
</style>
