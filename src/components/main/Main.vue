<template>
    <div>
       <news/>
        <sections/>
    </div>
</template>

<script>
    import news from "./news"
    import sections from "./sections"
    export default {
        name: "main.vue",
        components:{
            news,
            sections
        }
    }
</script>

<style scoped>

</style>