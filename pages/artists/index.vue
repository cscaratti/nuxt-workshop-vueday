<template>
    <div>
        <Navbar></Navbar>
        <ArtistPreview v-for="artist in artists" :key="artist.id" :artist="artist"></ArtistPreview>
    </div>
</template>

<script>
    import fakeData from '@/assets/artist-fake-data.js'
    import ArtistPreview from "@/components/ArtistPreview"
    import Navbar from "@/components/Navbar"

    export default {
        name: "index",
        components: {ArtistPreview, Navbar},
        data() {
            return {
                artists: fakeData
            }
        }
    }
</script>

<style scoped>

</style>