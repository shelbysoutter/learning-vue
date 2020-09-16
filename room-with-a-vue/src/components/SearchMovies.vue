<template>
    <div>
        <form @submit="searchMovies">
            <input type="text" v-model="title" name="title" placeholder="Search...">
            <input type="submit" value="Search">
        </form>
    </div>
</template>

<script>
export default {
    name: "SearchMovies",
    data() {
        return {
            title: ''
        }
    },
    methods: {
        searchMovies() {
            
        }
    }
}
</script>

<style scoped>

</style>