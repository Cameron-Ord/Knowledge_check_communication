<template>
    <div class="parent">

        <span class="profile_span">

            <h1>{{ user[`name`] }}</h1>

            <p> {{ user[`is_premium`] }}</p>

            <h5 v-if="user[`is_premium`] === true ">PREMIUM USER</h5>

            <p v-else>BASIC</p>

            <button @click="user_click" >CLICK ME</button>

        </span>

    </div>
</template>

<script>
    export default {
        

        props: {


            user: Object,


        },


        methods:{

            user_click(){

                this.$emit(`user_click`, this.user[`id`]);
            }

        }
    }
</script>

<style scoped>

</style>