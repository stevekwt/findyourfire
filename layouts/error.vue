<template>
    <div>
        <div class="container">
            <PageNotFound />
        </div>
    </div>
</template>

<script>
import PageNotFound from "../components/PageNotFound.vue";
    export default {
    components: { PageNotFound }
}
</script>

<style scoped>
    .container {
        padding: 4rem 0;
    }
</style>