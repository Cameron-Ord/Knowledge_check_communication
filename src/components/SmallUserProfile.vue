<template>
    <div class="parent">

        <span class="profile_span">

            <h1>{{ user[`name`] }}</h1>

            <p> {{ user[`is_premium`] }}</p>

        </span>

    </div>
</template>

<script>
    export default {
        

        props: {


            post: Object


        }
    }
</script>

<style scoped>

</style>