<template>
    <main>
        <Nav/>
        <section>
            <Sidebar/>
            <div class="content">
                <router-view/>
            </div>
        </section>
    </main>
</template>
<script>
    import Nav from "../containers/Nav";
    import Sidebar from "../containers/Sidebar";

    export default {
        name: 'Layout',
        components: {Sidebar, Nav}
    }
</script>
<style lang="scss">
    main{
    height:100vh;
        display: flex;
        flex-direction: column;
    }
    section{
        flex:1;
        width:100%;
        display: flex;
        .side-bar{
            height:100%;
            width:20%;
            box-shadow: 0 2px 8px rgba(0,0,0,0.12);
        }
        .content{
            flex:1;
        }
    }
</style>
