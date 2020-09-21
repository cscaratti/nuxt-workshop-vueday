<template>
    <div>
        <Navbar></Navbar>
        <h2>{{ $route.params.id }}</h2>
    </div>
</template>

<script>
    import Navbar from "@/components/Navbar"

    export default {
        name: "_id",
        components: { Navbar }
    }
</script>

<style scoped>

</style>