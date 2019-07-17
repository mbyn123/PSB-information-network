<template>
    <div>
        <Head/>
        <Nav/>
        <Mains/>
    </div>
</template>

<script>
    import Head from "../Head"
    import Nav from "../Nav"
    import Mains from "../mains/Mains"
    export default {
        name: "component.vue",
        components:{
            Head,
            Nav,
            Mains
        }
    }
</script>

<style scoped>


</style>