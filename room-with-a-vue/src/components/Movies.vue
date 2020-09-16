<template>
    <div>
        <div v-bind:key="movie.id" v-for="movie in movies">
            <MoviePhoto v-bind:movie="movie"/>
        </div>
    </div>
</template>

<script>
import MoviePhoto from './MoviePhoto.vue';

export default {
    name: "Movies",
    components: {
        MoviePhoto
    },
    props: ["movies"]
}
</script>

<style scoped>

</style>