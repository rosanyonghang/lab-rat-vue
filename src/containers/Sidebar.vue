<template>
    <div class="side-bar">
        <div class="side-bar-item">Home</div>
        <div class="side-bar-item">About</div>
        <div class="side-bar-item">Services</div>
        <div class="side-bar-item">Products</div>
        <div class="side-bar-item">Contacts</div>
    </div>
</template>
<script>
    export default {
        name: 'Sidebar'
    }
</script>
<style lang="scss">
    .side-bar-item {
        padding: 10px 0px 10px 5vw;
        background: white;
        transition: .3s;
        cursor: pointer;
        &:hover {
            filter:brightness(.95);
        }
    }
</style>
