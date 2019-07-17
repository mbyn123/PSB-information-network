<template>
    <div>
        <Head/>
        <Nav/>
        <Main/>
    </div>
</template>

<script>
    import Head from "../Head"
    import Nav from "../Nav"
    import Main from "../main/Main"
    export default {
        name: "component.vue",
        components:{
            Head,
            Nav,
            Main
        }
    }
</script>

<style scoped>


</style>