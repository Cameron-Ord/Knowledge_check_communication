<template>
  <div class="omega_parent">
    <header class="page_header">


    </header>
    <main class="page_main">
      <section>
        <article>
          <span v-for="user in users" :key="user" :post="user" class="user_profile">

            <h1>{{ user[`name`] }}</h1>

            <p>{{ user[`age`] }}</p>

            <p>{{ user[`is_premium`] }}</p>

            <p>{{ user[`id`] }}</p>

          </span>
        </article>
        <article>

          <small-user-profile></small-user-profile>

        </article>
      </section>
    </main>
    <footer class="page_footer">


    </footer>
  </div>
</template>

<script>

import SmallUserProfile from './components/SmallUserProfile.vue';

export default {


  data() {
    return {
      users: [{



        name: `Cameron`,

        age: `25`,

        is_premium: true,

        id: 327623

      },


      {


        name: `James`,

        age: `29`,

        is_premium: true,

        id: 219823



      },

      ]
    }
  },





  name: 'App',
  components: {

    SmallUserProfile

  },




}
</script>

<style></style>
